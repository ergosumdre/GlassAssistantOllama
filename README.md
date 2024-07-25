# GlassAssistant

Use LLava Vision from Ollama and OpenAI's Transcription capabilities to understand the world around you.

## Setup
1. Download and install Tailscale on your hosted Ollama machine and your Google Glass from F-Droid.
2. Edit line 162 on app/src/main/java/dev/synople/glassassistant/fragments/LoadingFragment.kt with your Tailscale Host IP Address ie: XXX.XXX.XX.XXX:11434/api/generate/
3. Start Ollama on your host machine with the following args: OLLAMA_HOST=XXX.XXX.XX.XXX:11434 ollama serve
4. Generate an OpenAI API Key: https://platform.openai.com/api-keys.
5. Turn the API Key into a QR Code.
6. Install and launch the GlassAssistant app on Glass.
7. Scan the generated QR Code.
8. Hold the camera button and speak for a custom prompt. Otherwise tap Glass to use a default prompt.
9. The results are vertically scrollable. Tap Glass or click the camera button to return to the Camera view.


## Screenshots
![A diecast model car is visible through Glass EE2 with application usage instructions on screen.](./README/camera.png)

![A transcription of the spoken text is visible, with a loading animation underneath](./README/loading.png)

![White text on a black background: The primary object in the image is a small replica of a vintage convertible car, possibly a collectible or a toy, displayed on a wooden surface with a purple light illuminating the background.](./README/result.png)
