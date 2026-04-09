# AI-Assisted Customization Platform Prototype

## Overview

This repository contains the front-end implementation of the AI-assisted customization platform utilized in the experimental studies for the manuscript "When AI-Assisted Customization Outperforms Self-Directed Customization in Digital Luxury Contexts: The Role of Design Freedom". 

The codebase provides an interactive web interface that simulates a digital luxury customization experience. It integrates two distinct artificial intelligence models to process consumer input and generate unique visual outputs. The system first utilizes a Large Language Model to refine consumer text prompts into standardized design instructions, which are subsequently processed by a latent text-to-image diffusion model to generate the final customization artifact.

This code is provided as open-source exploratory support to facilitate academic transparency, replication, and early-stage experimentation. It serves as a proof-of-concept prototype rather than a scalable, production-ready enterprise solution.
## Persistent Identifier

 DOI: 10.5281/zenodo.19479056 
 
## Prerequisites and Configuration

To deploy and execute this prototype locally, the following external API dependencies must be configured:

1. Doubao API Key: Required for the prompt refinement process. Obtainable via the Volcengine console.
2. Stability AI API Key: Required for the Stable Diffusion image generation process. Obtainable via the Stability AI developer platform.

### Implementation Instructions

1. Download or clone this repository to your local environment.
2. Open the `index.html` file in a standard text editor.
3. Locate the API Configuration section within the JavaScript block.
4. Replace the placeholder string `YOUR_DOUBAO_API_KEY_HERE` with your active Volcengine API key.
5. Replace the placeholder string `YOUR_STABILITY_AI_API_KEY_HERE` with your active Stability AI API key.
6. Provide a local path or valid URL for the base product image by modifying the `src` attribute of the `<img class="tshirt-base">` tag.
7. Save the modifications and open `index.html` in a modern web browser to interact with the prototype.

## System Architecture

The prototype is consolidated into a single file to ensure straightforward deployment.

HTML Structure: Establishes the user interface, comprising an input section for text prompts and a dynamic preview section for visualizing the generated design overlaid on a base product template.
CSS Styling: Employs a minimalist aesthetic aligned with standard digital luxury interfaces, ensuring responsive behavior across varying screen dimensions.
JavaScript Logic: Manages asynchronous requests to the external generation APIs, handles error states, and dynamically manipulates the Document Object Model to display the generated base64 image data.
