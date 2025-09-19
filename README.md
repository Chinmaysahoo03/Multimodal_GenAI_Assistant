# Multimodal Generative AI Assistant

A unified conversational AI system using LangChain with Groq for LLM inference and Hugging Face Stable Diffusion for text-to-image generation. Supports stateful chats and on-the-fly image creation from prompts or responses, all in Google Colab.

## Features
- **Conversational AI**: Stateful dialogue with Groq's Gemma-2-9B-IT via LangChain.
- **Text-to-Image**: Generates images using Stable Diffusion with prompt engineering.
- **Integration**: Command-based (e.g., "generate image: [prompt]") for seamless multimodal interaction.
- **Optimization**: GPU-accelerated, cost-free (free Groq tier, open-source models).
- **Deployment**: Fully runnable in Colab; exportable to apps.

## Tech Stack
- **Languages/Frameworks**: Python, LangChain-Groq, Diffusers.
- **LLM**: Groq Gemma-2-9B-IT.
- **Image Gen**: Hugging Face Stable Diffusion v1-4.
- **Requirements**: Groq API key, Torch (GPU recommended).

## Installation
1. Clone the repo:

2. In Google Colab:
- New notebook, copy cells.
- Install: `!pip install langchain-groq langchain transformers torch diffusers accelerate pillow`
3. Set Groq API Key: Colab Secrets > `GROQ_API_KEY`.
4. Enable GPU: Runtime > Change runtime type > T4 GPU.

## Usage
1. Run Cells 1-2 for setup.
2. Test Chat (Cell 3): Standalone response generation.
3. Test Image (Cell 4): Generate from prompt.
4. Interactive Mode (Cell 5): Chat and generate images (e.g., "generate image: a cat").
5. Demo (Cell 6): Scripted example.

Example:

You: Hi, what's generative AI?
Assistant: Generative AI is a type of artificial intelligence that can create new content, like text, images, music, code, or even 3D models. 

Think of it like this: instead of just analyzing existing data, generative AI learns the patterns and rules behind that data and then uses that knowledge to generate something entirely new. 

Here are some examples:

* **Text:** ChatGPT (that's me!), can write stories, poems, articles, and even code based on your prompts.
* **Images:** DALL-E 2 can create realistic images from your text descriptions, like "a cat wearing a hat riding a unicorn."
* **Music:** AI systems can compose original music in different styles.
* **Code:** AI can help generate code in various programming languages.

Generative AI is still a rapidly developing field, but it has the potential to revolutionize many industries, from art and entertainment to healthcare and education.


Let me know if you have any other questions! 😊
---

You: Can you describe a scene of AI creating art?
Assistant: Imagine a dimly lit studio, bathed in the soft glow of multiple monitors. In the center, a sleek machine hums quietly, its fans whirring like a gentle breeze. This isn't a traditional artist's studio, though. There are no canvases, no paintbrushes, no sculptures taking shape from clay. Instead, there are lines of code scrolling across the screens, complex mathematical formulas dancing in a digital ballet. 

This is where AI creates its art. 

On one screen, a user inputs a prompt: "A lone astronaut gazing at a nebula, painted in the style of Van Gogh." The AI, a sophisticated neural network, digests this information, analyzing the concepts, the emotions, the artistic style. It draws upon a vast library of images, paintings, and even musical compositions, learning the patterns, the brushstrokes, the color palettes that define these different artistic expressions.

Within the machine, a symphony of calculations unfolds. Algorithms sift through data, identifying relationships between colors, shapes, and textures. The AI begins to weave a tapestry of pixels, generating an image that embodies the user's prompt. 

As the process progresses, the screen fills with a swirling vortex of colors, a cosmic landscape taking shape. The lone astronaut, rendered in a style reminiscent of Van Gogh's signature brushwork, stands silhouetted against the vibrant nebula, their gaze lost in the immensity of space.

Finally, the AI presents its creation. A breathtaking image, born not from a human hand, but from the mind of a machine. It's a testament to the power of artificial intelligence, its ability to not only analyze and understand, but to create something new, something beautiful, something uniquely its own.
---

--- Image Request: AI painting a masterpiece ---
<img width="512" height="512" alt="gen ai" src="https://github.com/user-attachments/assets/a29c6f1b-e6e2-434a-abd5-98649a773fc1" />



## Code Structure
- **Cell 1**: Dependencies.
- **Cell 2**: Imports, LLM/Stable Diffusion setup.
- **Cell 3**: Chat function.
- **Cell 4**: Image generation (optimized for speed).
- **Cell 5**: Interactive loop.
- **Cell 6**: Demo script.

## Performance Tips
- Use GPU for 10-20s image gen (reduce steps to 25 if needed).
- Short prompts for faster results.

## Contributing
Add enhancements (e.g., voice input) via PRs.

## License
MIT License.

## Contact
Chinmaya Sahoo – chinmayasahoo3210@gmail.com  
Explore Gen AI multimodal capabilities!
