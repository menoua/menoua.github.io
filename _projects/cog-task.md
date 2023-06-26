---
layout: project
title: CogTask
photo: /assets/cog-task.png
tag: cog-task
type: side
code: https://github.com/menoua/cog-task
docs: https://docs.rs/cog-task/latest/cog_task/
sort_key: 1001
subtitle: "General-purpose low-latency tool for designing cognitive tasks."
description: "An application written in Rust for designing and running cognitive
    psychology tasks/experiments, with the goals of being low-latency and 
    easy-to-use."
---

This tool provides an easy way to write and execute different types of 
interactive actions that are usually useful in experiments involving cognitive 
sciences. E.g., display an image/video, play sounds, show text, measure 
reactions to events (through key presses or clicks), measure action completion 
times, ask questions, etc. The existing tools for this purpose are either 
out-dated, closed-source, or written in a low-performance scripting language 
like javascript. This tool aims to be modern and performant, while at the same 
time maintaining ease-of-use.

To achieve native performance, this application is written in [Rust](
https://www.rust-lang.org/) using the [egui](https://github.com/emilk/egui) 
graphical framework. To generate a task, a description file in the rust object 
notation ([RON](https://github.com/ron-rs/ron); see "Tooling" section of its 
README for syntax highlighting) format should be created by the experiment 
designer. The task file consists of three main fields: name, configuration, 
and blocks (self-contained pieces of the experiment that should be run in one 
sitting). Each block in itself consists of three main fields: name, 
configuration (overriding the task configuration), and actions. The actions 
are specified in the form of a tree (graph) with nodes of type `Action`.

For usage examples and installation instructions see the GitHub [page](
{{ page.code }}).

___DISCLAIMER:___ _While this tool is functional and feature-rich, this project 
is highly experimental and its API is subject to frequent change. Use at your 
own risk._
