---
title: "Image Rotator"
description: A Rust-based WebAssembly application that allows users to upload and rotate images.
date: 2025-03-17 00:00:00 +0800
categories: [Personal Projects]
tags: [Rust, React, TypeScript, WebAssembly, Website]
---

## Information
Image Rotator is a Rust-based WebAssembly application that utilises the image crate to allow users to upload and rotate images. The front-end is handled by React. When the user uploads an image and clicks the “Print Dimensions” or “Rotate Image” function, the TypeScript front-end calls the relevant Rust back-end function. These back-end functions are dependent on various functions from Rust’s image crate.

I developed this little toy web app to improve my skills in Rust, which is a new language to me. I was taking a Rust course at uni at the time and I figured that I could best prepare myself for the first assignment through creating a toy app in my own time. I chose React for the front-end as its a web framework I enjoy coding in. The key takeaways from this experience were learning how to use Rust crates and Wasm-bindgen, which enables interactions between Rust and TypeScript.

## Features
- Upload an image and view its dimensions.
- Rotate an image to your preferred orientation.

## Source Code
[![View on GitHub](https://img.shields.io/badge/GitHub-View_repository-blue?style=for-the-badge&logo=github)](https://github.com/IssacMathai/Image-Rotator/)
