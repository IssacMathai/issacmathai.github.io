---
title: "Image Rotator"
description: A Rust-based WebAssembly application that allows users to upload and rotate images.
date: 2025-05-06 00:00:00 +0800
categories: [Personal Projects]
tags: [Rust, React, TypeScript, WebAssembly, Website]
---

## Information
Image Rotator is a Rust-based WebAssembly application that utilises the image crate to allow users to upload and rotate images. The front-end is handled by React. When the user uploads an image and clicks the “Print Dimensions” or “Rotate Image” function, the TypeScript front-end calls the relevant Rust back-end function. These back-end functions are dependent on various functions from Rust’s image crate.

I developed this little toy web app to improve my skills in Rust, which is a new language to me. I chose React for the front-end as its a web framework I enjoy coding in.

## Features
- Upload an image and view its dimensions.
- Rotate an image to your preferred orientation.

## Source Code
[![View on GitHub](https://img.shields.io/badge/GitHub-View_repository-blue?style=for-the-badge&logo=github)](https://github.com/IssacMathai/Image-Rotator/)
