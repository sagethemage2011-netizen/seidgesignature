Aloha! It's seidge, otherwise known as seidge the mage on X!

I have created a system of digitally watermarking my art so that you can verify if something is my art!

If you don't already have openstego, download it. Once you open it, go to "Verify watermark". Input my image in "File to be checked for watermark",
and the watermark file (Provided in the repo) in "Original signature file", then click "Verify watermark".

The image will give a watermark signal strength, which will still retain some information when it is cropped, copied, and lightly modified.

You can find OpenStego at openstego.com.

Edit: Before, the watermark would go away upon being edited by AI. Then, I decided to add some pure noise to my photos. You can find a noise generator at https://robson.plus/white-noise-image-generator/. All I had to to was add the noise to the image, set the noise to a low opacity, and then add the watermark to that image. The idea is that since random noise has more shannon entropy, it has more data, and thus, more data to be hid inside it. This makes digital watermarks more prominent in these images. Before, a watermark for a black and white image would be around 50% to 0% upon something edited with AI. Now, it jumped to something like a 70% to a 10% on an AI edited image, meaning it's still somewhat detectable!
