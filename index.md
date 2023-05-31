---
layout: home
subtitle: BrainTalker
---

<h2> BrainTalker: Low-Resource Brain-to-Speech Synthesis with Transfer Learning using Wav2Vec 2.0
</h2>

Submitted to IEEE BHI 2023

<h3>Authors
</h3>
Miseul Kim, Zhenyu Piao, Jihyun Lee and Hong-Goo Kang†

<h3>Github code
</h3>
<a href="https://github.com/braintalker/braintalker_pytorch">Braintalker_pytorch</a>

<br />

<h3>Proposed Method</h3>

Decoding spoken speech from neural activity in the brain is a fast-emerging research topic, as it could enable communication for people who have difficulties with producin audible speech. For this task, electrocorticography (ECoG) is a common method for recording brain activity with high temporal resolution and high spatial precision. However, due to the risky surgical procedure required for obtaining ECoG recordings, relatively little of this data has been collected, and the amount is insufficient to train a neural network-based Brain-to-Speech (BTS) system. To address this problem, we propose BrainTalker—a novel BTS framework that generates intelligible spoken speech from ECoG signals under extremely low-resource scenarios. We apply a transfer learning approach utilizing a pre-trained self-supervised model, Wav2Vec 2.0. Specifically, we train an encoder module to map ECoG signals to latent embeddings that match Wav2Vec 2.0 representations of the corresponding spoken speech. These embeddings are then transformed into mel-spectrograms using stacked convolutional and transformer-based layers, which are fed into a neural vocoder to synthesize speech waveform. Experimental results demonstrate our proposed framework achieves outstanding performance in terms of subjective and objective metrics, includinga Pearson correlation
coefficient of 0.9 between generated and ground truth mel-spectrograms. We share publicly available Demos and Code.

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
            <img src="./assets/img/e.png" width="200">
        </td>
        <td class="someting">
            <img src="./assets/img/f.png" width="200">
        </td>
        <td class="someting">
            <img src="./assets/img/g.png" width="200">
        </td>
        <td class="someting">
            <img src="./assets/img/h.png" width="200">
        </td>
    </tr>
    <tr>
        <td>
        	Synthesized Spectrogram
        </td>
        <td class="someting">
            <img src="./assets/img/e_t.png" width="200">
        </td>
        <td class="someting">
            <img src="./assets/img/f_t.png" width="200">
        </td>
        <td class="someting">
            <img src="./assets/img/g_t.png" width="200">
        </td>
        <td class="someting">
            <img src="./assets/img/h_t.png" width="200">
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
