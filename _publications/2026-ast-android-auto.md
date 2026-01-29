---
title: "Detecting Compliance Violations in Android Auto Applications"
collection: publications
category: conferences
permalink: /publication/2026-ast-android-auto
excerpt: 'This paper presents our approach to detecting compliance violations in Android Auto applications through static analysis techniques.'
date: 2026-05-01
venue: 'AST 2026 - IEEE/ACM International Conference on Automation of Software Test'
# slidesurl: 'http://academicpages.github.io/files/slides-ast2026.pdf'
# paperurl: 'http://academicpages.github.io/files/paper-ast2026.pdf'
# citation: 'Your Name, et al. (2026). &quot;Detecting Compliance Violations in Android Auto Applications.&quot; <i>AST 2026</i>.'
---

Android Auto provides a platform for running apps safely while driving, but ensuring apps comply with safety guidelines is challenging. This paper presents our approach to detecting compliance violations in Android Auto applications using static analysis.

## Abstract

Despite over 3.5 million Android apps and 200+ million Android
Auto-compatible vehicles, only a few hundred apps support Android
Auto due to platform-specific compliance requirements. Android
Auto mandates service-based architectures in which the vehicle system invokes app callbacks to render the UI and handle interactions,
which is fundamentally different from standard Activity-based Android development. Through an empirical study analysis of 98 issues
across 14 Android Auto app repositories, we identified three major
compliance failure categories: media playback errors, UI rendering issues, and voice command integration failures in line with
mandatory requirements for integrating Android Auto support. We
introduce AutoComply, a static analysis framework capable of
detecting these compliance violations through the specialized analysis of platform-specific requirements. AutoComply constructs a
Car-Control Flow Graph (CCFG) extending traditional control flow
analysis to model the service-based architecture of Android Auto
apps. Evaluating AutoComply on 31 large-scale open-source apps,
it detected 27 violations (13× more than Android Lint), while no
false positives were observed, achieving 2× faster analysis. Developers have acknowledged 14 of these violations with 8 fixes already implemented, validating AutoComply’s practical effectiveness.

## Key Contributions

- We present the first comprehensive study focused on understanding the challenges faced by developers in creating Android
Auto-compliant apps.
- We propose Car Control Flow Graph (CCFG), which models the
control flow specific to Android Auto apps based on the available
features in the apps.
- We developed a novel static analysis specifically designed to
identify compliance issues in Android Auto apps, including UI
issues and problems with media playback and voice command
integration.
- We evaluate AutoComply on real-world apps, showing its effectiveness by detecting 27 issues related to Android Auto compliance, 14 of which were confirmed by developers, and 8 of them
have already been fixed.

## Tools & Techniques

<!-- Our approach leverages taint analysis and callback-aware static analysis using tools like FlowDroid and SootUp to identify potential compliance issues. -->

For further reading, check it out on [arxiv](https://arxiv.org/abs/2503.04003v3).

<!-- Recommended citation: Your citation here -->
