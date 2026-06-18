---
title: "Visual Memory"
excerpt: "Click here for an introduction to my work on visual memory<br/><br/><img src='/images/memory.png'>"
collection: research1
---
How do we store incoming visual information from the world around us? It is easy to take for granted just how much information our minds hold onto from one moment to the next. Every time you move your eyes—which happens around 100,000 times a day—your brain briefly stores what you just saw so it can compare it with what you are looking at next. This cognitive system is known as visual working memory.
<br/><br/>
While scientists have studied visual working memory for decades, the vast majority of research relies on simplified artificial arrays—like a few colored squares on a gray screen. While highly controlled, these traditional experiments don't capture the messy, continuous, beautifully complex nature of the real world. In real-world scenes, colors fade gradually, shapes are irregular, and objects blend into one another.
<br/><br/>
To bridge this gap, Steve and I developed a new way to model how the human brain stores real-world visual scenes. Our model proposes that the working memory representation of a scene is simply a weaker, noisier echo of the brain's original perceptual representation in the ventral visual processing pathway. To test this, we used CORnet-S, a deep neural network (DNN) explicitly engineered to mirror the anatomical stages of the human visual cortex (from basic features in V1 to complex, abstract objects in IT).
<br/><br/>
<img src='/images/Picture1.svg'>
<br/><br/>
The results were incredibly striking! In our first experiment, our model accounted for a massive 76% of the variance in human response times across different scene pairs. It vastly outperformed basic pixel-level changes (which only explained 29%) and came remarkably close to matching the "ground truth" of explicit human ratings of visual similarity (78%).
<br/><br/>
<img src='/images/Picture4.svg'>
<br/><br/>
We even tested it on focal changes where an entire object was seamlessly added or deleted from a photograph using Photoshop. After modifying the network to account for "center bias"—the human tendency to focus on the middle of a image—the model continued to successfully predict how well a human subject would be able to detect specific object changes.
<br/><br/>
Predicting behavior is one thing, but does the model actually mirror what the brain is doing while it is actively remembering? To answer this, we recorded electrical brain activity using EEG while participants held a real-world scene in their working memory.
Using a technique called Representational Similarity Analysis (RSA), we compared the geometric relationships of the neural patterns recorded from the scalp directly to the population vectors inside our deep neural network model. Right on cue, during the crucial delay period when the image was missing from the screen, the patterns of voltage across the scalp closely matched the representational geometry of the model's visual areas. This provides direct, neural evidence that our model is successfully capturing the actual format the brain uses to store the real world in mind.
<br/><br/>
<img src='/images/Picture5.svg'>
<br/><br/>
### [Kiat, J. E., & Luck, S. J. (2026). A population vector model of visual working memory for real-world scenes. Journal of Experimental Psychology: General](https://psycnet.apa.org/doi/10.1037/xge0001921){:target="_blank"}
