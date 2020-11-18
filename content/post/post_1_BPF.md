---
date: 2020-11-17T11:25:05-04:00
description: "Dynamics 365"
featured_image: "/images/bpf.png"
tags: [Dynamics 365]
title: "Intro to Business Process Flow (BPF)"
disable_share: false
---
Dynamics 365 has the added bonus of incorporationg the most inportant parts of the Business Logic, no matter what that might be. Often is not this tool the challanging part but rather the identifying of Business critical information to include in the Process it self. In this Post we will however only focus on the technical part of the BPF.

{{< figure src="/images/bpf_stage_condition.png" title="Illustration of configuration UI 1. Stage 2. Condition" >}}

A BPF is devided into Stages and each stage may hold Data Steps of different types, most often field that has been added to the Entity (or Table as Microsoft as named it now). 

{{< figure src="/images/bpf_components.png" title="Illustration of configuration UI with all components" >}}

The first stage of a BPF is related to the entity and can not be related to a different entity or be influensed by any logic operator, with in the BPF it self, Business Rules on the form may still influence. A logic operation in the BPF is basically branching and is performed by Conditions of one or more [AND] or [OR] conditions. 

{{< figure src="/images/bpf_logic_properties.png" title="Illustration of configuration UI 1. Stage 2. Condition" >}}

When a condition is configured with more than one Rule, the configurator has to choose between [AND] or [OR] as stated above, and this means that coplexity of evaluation rules are reduced.

As conclusion for this intro it should be clear that we have great flexibility when we select the information and most logics can be solved here. But as with any system there are limitations to what the system is capable of, and we will cover some more limitations in the system related to number of stages and conditions in a later stage.

As an exiting last point before wraping up is that the inclution of a Microsoft Flow Data Step in the BPF really gives the BPF endles posibilities. As of writing it is still in preview, meaning that Microsoft has no support of it and it should not be used in Production... but we can still play.