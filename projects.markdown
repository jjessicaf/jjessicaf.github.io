---
layout: default
title: Projects
nav_order: 3
description: "Projects"
permalink: /projects/
---

<h1>You can check out some of my tech projects below.</h1>

<h2>Emote Recommender</h2>
[presentation](https://docs.google.com/presentation/d/1-vDMK1vmKV7w2So8sbAKd6_02oleM0RGWwuZ70pL-uc/edit?usp=sharing)

<h3>Motivation</h3>
<ul>
    <li>NLP on online livestream conversations needs further exploration</li>
    <li>Important to understand and analyze language used in online communication</li>
    <li>Twitch offers documentations of these live conversations</li>
    <li>Understand impact of social media and anonymity on communication</li>
</ul>
<h3>Data</h3>
<ul>
    <li>Chat logs of past stream videos (VODs) from Twitch streamer Joe Bartolozzi</li>
    <li>Removed timestamps, usernames, bot commands, mentions, and links</li>
    <li>Roughly 37,000 lines of chat from 8 VODs</li>
    <li>Labeled with one of five labels: joebartbusiness, joebartlongneck, joebartwebelieve, lul, catjam</li>
</ul>
<h3>Methods</h3>
<ul>
    <li>Labeled chat rows used to fine-tune Bidirectional Encoder Representations from Transformers (BERT) base model</li>
    <li>To address overfitting we froze all embeddings layers and first five encoding layers</li>
    <li>Trained model used for classification on new individual lines of chat data</li>
</ul>
<h3>Results</h3>
<ul>
    <li>Accuracy: 0.84</li>
    <li>Precision: 0.75</li>
    <li>Recall: 0.27</li>
    <li>F1-score: 0.37</li>
    <li>AUROC:
    <ul>
        <li>joebartbusiness: 0.73298</li>
        <li>joebartlongneck: 0.71129</li>
        <li>joebartwebelieve: 0.7687</li>
        <li>lul: 0.74796</li>
        <li>catjam: 0.85962</li>
    </ul>
</ul>
<h3>Conclusion</h3>
<ul>
<li>In-person and online communication differ:</li>
<ul>
    <li>Online platforms afford anonymity</li>
    <li>Presence of different language patterns</li>
    <li>Can extend to future research regarding online communication</li>
</ul>
<li>Help understand the impact of these online communities on sensitive topics</li>
<li>Future steps:</li>
<ul>
    <li>Scale up data volume: more Twitch communities and more diverse genres</li>
    <li>Expanding the model beyond classification to reveal patterns in content and speech of various communities</li>
</ul>
</ul>
<h3>Poster</h3>
You can find the poster for this project below, or at the following [link](https://github.com/jjessicaf/CAIS-Proj-Emote/blob/main/readme/Emote_recommender_poster.pdf).
