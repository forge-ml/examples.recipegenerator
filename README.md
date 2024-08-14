# Recipe Generator

This is a recipe generator application built with Forge. It allows users to upload images and generate recipes based on those images using ChatGPT.

## How it works

1. Users upload an image to Amazon S3.
2. The uploaded image is displayed in a carousel.
3. When the user presses the "Generate" button, the forge makes a call to ChatGPT.
4. ChatGPT analyzes the image and generates a structured recipe response fitting the recipe.ts schema.
5. The generated recipe is displayed on the screen.

##Why use Forge?

If you try making an app like this an issue you run into is that chatGPT can return any type of response. However, with forge you can define a schema and the response will be validated against that schema. This way you can be sure that the response you get back will always be in the correct format. This makes integrating chatGPT responses into your app seamless and effective.

Live Site: https://forge-recipegenerator.onrender.com/

If you want to try it for yourself:

git clone https://github.com/forge-ml/examples.recipegenerator
npm i
npm run dev
