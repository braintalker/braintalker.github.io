---
layout: home
subtitle: BrainTalker
---

<h2> BrainTalker: Low-Resource Brain-to-Speech Synthesis with Transfer Learning using Wav2Vec 2.0
</h2>

Submitted to INTERSPEECH 2023 (Paper ID: 2233)

<h3>Authors
</h3>

Anonymous submission

<br />

<h3>Proposed Method</h3>
<img src="./assets/img/proposed.png" width="1000">

In this paper, we propose BrainTalker – a novel brainto-speech synthesis framework that generates intelligible spoken speech from electrocorticography (ECoG) signals under an
extremely low-resource scenario. Despite its high-resolution
strength, ECoG requires a risky surgical procedure that severely
limits the data collection. To solve this problem, we propose
a transfer learning approach that utilizes a pre-trained selfsupervised model Wav2Vec 2.0 and extracts generalized latent
features from the ECoG signals. Also, we introduce context
loss, a novel loss function that reduces the information gap
between the brain and speech representations obtained from
Wav2Vec 2.0 respectively. We feed the extracted representations into a mel generator and synthesize mel spectrograms for
speech waveform generation. Our experimental results show
that BrainTalker can generate natural and intelligible speech in
terms of both subjective and objective metrics. We release the
demo page and code publicly

<br />

<h3>Samples
</h3>


<table style="margin-left: auto; margin-right: auto;">
    <tr>
        <td>
        	GT Spectrogram
        </td>
        <td class="someting">
            <img src="./assets/img/a_gt.png" width="300">
        </td>
        <td class="someting">
            <img src="./assets/img/b_gt.png" width="300">
        </td>
        <td class="someting">
            <img src="./assets/img/c_gt.png" width="300">
        </td>
        <td class="someting">
            <img src="./assets/img/d_gt.png" width="300">
        </td>
    </tr>
    <tr>
        <td>
        	Synthesized Spectrogram
        </td>
        <td class="someting">
            <img src="./assets/img/a_syn.png" width="300">
        </td>
        <td class="someting">
            <img src="./assets/img/b_syn.png" width="300">
        </td>
        <td class="someting">
            <img src="./assets/img/c_syn.png" width="300">
        </td>
        <td class="someting">
            <img src="./assets/img/d_syn.png" width="300">
        </td>
    </tr>
    <tr>
        <td class="first-col">Ground Truth</td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/F03_B01_S36_R02_N_target.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/F03_B02_S13_R02_N_target.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/F03_B03_S21_R02_N_target.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/F03_B07_S07_R01_N_target.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">Baseline</td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/baseline/F03_B01_S36_R02_N.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/baseline/F03_B02_S13_R02_N.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/baseline/F03_B03_S21_R02_N.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/baseline/F03_B07_S07_R01_N.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">Proposed</td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/F03_B01_S36_R02_N.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/F03_B02_S13_R02_N.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/F03_B03_S21_R02_N.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/F03_B07_S07_R01_N.wav"></audio></td>
    </tr>
</table>

<br />