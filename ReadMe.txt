Intro:  

Generative Diffusion Models are models capable of generating images based on random noise. These models have risen in popularity due to their ability to produce large varieties of high-quality images.
Generative diffusion models work by iteratively adding noise to images gradually reducing the visual data in the image, this is called a forward process. A model can then be trained to undo the generated noise based on the image and timestep, this is referred to as a backward process. Afterwards the model can be prompted with random noise to create an entirely new image.  

 

Goal:  

The goal in this project is to explore the field of generative models and Generative Diffusion. This will be done through the creation of a small diffusion model, capable of producing 24X24 pixel sized images of cats.   

  

Motivation:  

As previously stated, the main goal of this project is to learn about generative diffusion models, and generating images is a means to do so.  Currently there exists many powerful models (such as Dalle-3, Midjourney, and Stable Diffusion) capable of generating high quality, realistic images.
Generative models utilizing diffusion are not limited to creating images and can also be modified to produce different types of data. Such as generating videos, audio (music), creating 3D models used in manufacturing to reduce cost, improve safety or boost efficiency. 

 Diffusion can provide a cheap way to generate high quality game assets, such as creating textures, normal maps and meshes for game production​ (Poole, 2022)​. For healthcare diffusion can enrich datasets as well as upscale images. 

While generating images of cats might not be too useful by itself, Diffusion can have the potential to enhance efficiency, reduce costs and produce high quality data for a vast number of industries.   

 

Execution of the program: 

The core for this project is the DDPM_cats.ipynb file.   

It contains the executive code for the project and details of how the system processes images, generates noise and iterates through the training loop. The initial part of the system handles preprocessing of data and contains various models for visualization of the images.
The center part describes the initialization of the model, initializes the model and trains it.  Lastly the final part displays the results of the model and provides a Gradio interface equipping the user with the ability to generate their own images.  

 

 

Another file provided is the model.pt file. It contains a pre-trained model, trained by the group. Training the Diffusion model requires significant computational resources, therefore a trained model is provided to reduce the program's processing time.  
The final result of the model can be visualized using the gradio interface in the last cell of the program 

The execution of the code will generate a file with the name new_model.pt that stores the model with the lowest loss throughout the training process.   

The project also contains .gif files used for visualization purposes 

The training data is available in the cats_large/cats folder

 

Notes about the project:  

Parts of the code and the system is based on the work of​ (Pulfer, 2022)​ and ​(Ho, 2006)​ 

The diffusion model was trained on a graphics card of the type: NVIDIA GeForce RTX 4070 Laptop GPU for 17 epochs. Due to the model's computational cost, it's recommended to use a GPU for training. Training of the model was done locally, using Jupyter Notebook.  

 

  

 

 

​​References 

​​Ho, J., 2006. Denoising Diffusion Probabilistic Models, s.l.: arXiv. 

​Poole, B., 2022. github. [Online]  
Available at: https://dreamfusion3d.github.io/ 
[Accessed 18 3 2024]. 

​Pulfer, B., 2022. medium.com. [Online]  
Available at: https://medium.com/@brianpulfer/enerating-images-with-ddpms-a-pytorch-implementation-cef5a2ba8cb1 
[Accessed 18 3 2024]. 

​Rogge, N., 2022. huggingface. [Online]  
Available at: https://huggingface.co/blog/annotated-diffusion 
[Accessed 18 3 2024]. 

​​​ 
