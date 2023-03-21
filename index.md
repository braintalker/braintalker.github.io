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

<h3>Github code
</h3>
https://braintalker.github.io

<br />

<h3>Proposed Method</h3>
<img src="./assets/img/proposed.png" width="3000">

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
demo page and code publicly.

<br />

<h3>Seen samples
</h3>

<table style="width:10; height:10">
    <tr>
        <td>
        	GT Spectrogram
        </td>
        <td class="someting">
            <img src="./assets/img/a.png" width="200">
        </td>
        <td class="someting">
            <img src="./assets/img/b.png" width="200">
        </td>
        <td class="someting">
            <img src="./assets/img/c.png" width="200">
        </td>
        <td class="someting">
            <img src="./assets/img/d.png" width="200">
        </td>
    </tr>
    <tr>
        <td>
        	Synthesized Spectrogram
        </td>
        <td class="someting">
            <img src="./assets/img/a_t.png" width="200">
        </td>
        <td class="someting">
            <img src="./assets/img/b_t.png" width="200">
        </td>
        <td class="someting">
            <img src="./assets/img/c_t.png" width="200">
        </td>
        <td class="someting">
            <img src="./assets/img/d_t.png" width="200">
        </td>
    </tr>
    <tr>
        <td class="first-col">GT</td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/gt/HSH2_sem2_ecog_4_0.wav"></audio></td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/gt/HSH2_sem2_ecog_9_4.wav"></audio></td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/gt/HSH2_sem8_ecog_14_9.wav"></audio></td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/gt/HSH2_sem7_ecog_7_11.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">GT (hifi-gan)</td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/gt_hifigan/HSH2_sem2_ecog_4_0_target.wav"></audio></td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/gt_hifigan/HSH2_sem2_ecog_9_4_target.wav"></audio></td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/gt_hifigan/HSH2_sem8_ecog_14_9_target.wav"></audio></td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/gt_hifigan/HSH2_sem7_ecog_7_11_target.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">Proposed</td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/prop/HSH2_sem2_ecog_4_0.wav"></audio></td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/prop/HSH2_sem2_ecog_9_4.wav"></audio></td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/prop/HSH2_sem8_ecog_14_9.wav"></audio></td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/prop/HSH2_sem7_ecog_7_11.wav"></audio></td>
    </tr>
</table>

<br />

<h3>Unseen samples - [sʰon]
</h3>

<table style="width:10; height:10">
    <tr>
        <td>
        	GT Spectrogram
        </td>
        <td class="someting">
            <img src="./assets/img/a_gt.png" width="200">
        </td>
        <td class="someting">
            <img src="./assets/img/b_gt.png" width="200">
        </td>
        <td class="someting">
            <img src="./assets/img/c_gt.png" width="200">
        </td>
        <td class="someting">
            <img src="./assets/img/d_gt.png" width="200">
        </td>
    </tr>
    <tr>
        <td>
        	Synthesized Spectrogram
        </td>
        <td class="someting">
            <img src="./assets/img/a_syn.png" width="200">
        </td>
        <td class="someting">
            <img src="./assets/img/b_syn.png" width="200">
        </td>
        <td class="someting">
            <img src="./assets/img/c_syn.png" width="200">
        </td>
        <td class="someting">
            <img src="./assets/img/d_syn.png" width="200">
        </td>
    </tr>
    <tr>
        <td class="first-col">GT</td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/gt/HSH2_sem7_ecog_13_8.wav"></audio></td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/gt/HSH2_sem4_ecog_17_8.wav"></audio></td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/gt/HSH2_sem4_ecog_2_8.wav"></audio></td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/gt/HSH2_sem8_ecog_11_8.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">GT (hifi-gan)</td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/gt_hifigan/HSH2_sem7_ecog_13_8_target.wav"></audio></td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/gt_hifigan/HSH2_sem4_ecog_17_8_target.wav"></audio></td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/gt_hifigan/HSH2_sem4_ecog_2_8_target.wav"></audio></td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/gt_hifigan/HSH2_sem8_ecog_11_8_target.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">Proposed</td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/prop/HSH2_sem7_ecog_13_8.wav"></audio></td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/prop/HSH2_sem4_ecog_17_8.wav"></audio></td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/prop/HSH2_sem4_ecog_2_8.wav"></audio></td>
        <td><audio controls style="width: 200px;" preload="none"><source src="./assets/sample/prop/HSH2_sem8_ecog_11_8.wav"></audio></td>
    </tr>
</table>

<br />