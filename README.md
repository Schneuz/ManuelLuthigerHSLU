Audioreactive Video Rendering
Explore the cutting-edge world of audio reactive video creation using the powerful AI tool, Deforum. 

Step 1: Creating Videos with Deforum's Stable Diffusion Extension
Unleash the potential of Deforum, a video creation extension for Stable Diffusion, to generate captivating videos. Experiment with various parameters to achieve the desired visual effects. Deforum documentation is here: https://github.com/deforum-art/deforum-stable-diffusion . There is also a helpful Discord server: https://discord.com/invite/deforum 
Problem:
Encounter extended rendering times during the video creation process, hindering the efficiency of the project.
Solution:
Address the rendering time challenge by adopting a different model - TurboVisionXL SuperFastXLBasedOnNew_tvxlV20Bakedvae.safetensors [05b97497e5]. This model allows to produce high-quality images with only four steps and a CFG 2 configuration, significantly reducing the overall rendering time.

Step 2: Audioreactivity with Dynamic Keyframes
To create the audioreactive experience in our videos, I have employed a specialized audio keyframe generator from https://www.chigozie.co.uk . This tool allows us to dynamically generate keyframes based on audio amplitude, providing a foundation for synchronizing visuals with sound. In this step, we explore the integration of these keyframes into Deforum's Zoom function to create a audio reactive zoom effect.
Audio Keyframe Generation:
 
Utilize the audio keyframe generator from https://www.chigozie.co.uk  to generate keyframes. Ensure that the frames per second (FPS) align with the settings in Deforum for seamless integration.
Keyframe Integration with Deforum Zoom Function:
Implement the generated keyframes into Deforum's Zoom function. Experiment with different parameters to fine-tune the correlation between audio amplitude and the zoom effect. However the result was not that great so I searched for a better solution.
Step 3: Deforum Projects with Parseq
In our ongoing quest for creating compelling audioreactive videos, we introduce Parseq—a powerful tool for managing Deforum projects. Parseq enhances project organization, provides visualizations of key values, and facilitates easy adjustments for a more structured and efficient workflow.
Helpful Informations:
Parseq Documentation: Familiarize yourself with Parseq using the documentation available at https://github.com/rewbs/sd-parseq#readme . This resource serves as a comprehensive guide to harness the full potential of Parseq in Deforum projects.
Seed Management: Ensure video stability by managing the image seed in Parseq. By incrementing the seed for each keyframe, you can maintain visual consistency, creating a more stable output video.
Math Functions for Value Adjustment: Leverage Parseq's support for math functions to dynamically adjust values such as zoom, strength, etc. This flexibility allows for precise control over parameters, contributing to the overall refinement of the audioreactive effects. There is also a graph that shows the values over time. 
 
 

Time Series Integration: Explore the powerful Time Series feature in Parseq, enabling the import of any series of numbers. This functionality is particularly useful for syncing parameter changes to audio pitch or amplitude, enhancing the synchronization between visuals and audio cues.



Reference Audio Utilization: Improve alignment by loading a reference audio file into Parseq. Visualize its waveform alongside parameter graphs, making it easier to sync keyframes with audio events. Extracting key events, especially from stems like the snare drum, produces optimal results with minimal noise. You can automatically detect events and reference them in the math functions. 
 
AI Tools for Audio splitting: If access to stems is limited, employ AI tools like Reffusion & Ngrok to extract different instruments. This approach helps to get a clean and focused reference audio, enhancing the precision of key event extraction.
Helpful Tutorial: Robin Fernandes the founder of Parseq has a great youtube channel with some awesome tutorials: https://www.youtube.com/@rewbs 



