---
layout: about
title: about
permalink: /
subtitle: >
  Master Student · <a href="https://www.hiroshima-u.ac.jp/en" target="_blank">Hiroshima University</a> ·
  <a href="https://chikaraishi-lab.com" target="_blank">Urban and Transportation Planning Laboratory</a>

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>Higashihiroshima, Hiroshima, Japan</p>

news: true # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page
---

Every city planner faces a deceptively hard question: does this transport policy make residents better or worse off, and by how much? Answering it properly requires tracking how each person restructures their entire day in response to policy changes — not just aggregate travel-time savings.

Activity-based dynamic discrete choice models (DDCM) can capture this individual-level behavioural realism and derive rigorous welfare measures. The barrier is computational: exact estimation at realistic city scale demands ~1,000 CPU-days, and existing approximations from reinforcement learning and deep learning corrupt the welfare figure in ways that cannot be quantified.

My research develops **Structural Inverse Reinforcement Learning (Structural-IRL)**, an algorithm that resolves this barrier by exploiting two proven mathematical connections — between DDCM estimation and inverse reinforcement learning, and between DDCM backward induction and graph neural networks. These connections, made exact, yield tractable welfare measurement without approximation error. The result: for a policy like a new bus rapid transit corridor, Structural-IRL can estimate — for each household in the city — the net change in daily well-being, and identify which neighborhoods gain, which lose, and where complementary measures are most needed.

This research is conducted at the Urban and Transportation Planning Laboratory, [Hiroshima University](https://www.hiroshima-u.ac.jp/en), under the supervision of [Prof. Makoto Chikaraishi](https://chikaraishi-lab.com). The approach grew from master's thesis work, where exact estimation of a 10-parameter activity-based model on real Higashi-Hiroshima travel diary data (825 persons) was completed in ~17 hours on a GPU.
