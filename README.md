# Recipe Nutrition Analyzer

A web application that calculates nutrition facts and meal pattern crediting for recipes using the USDA FoodData Central API.

## Features

- 🥗 Calculate nutrition facts per serving using USDA database
- 📊 Display meal pattern crediting (fruits, vegetables, grains, etc.)
- ✏️ Manually add and edit ingredients with various units
- 🔄 Reset and start over
- 📏 Support for multiple measurement units (oz, lbs, grams, cups, tbsp, tsp, ml, l)

## Setup

1. **Start the development server**:
   ```bash
   npm start
   ```
   
   Or use npx directly:
   ```bash
   npx http-server -p 3000 -o
   ```

2. **Open your browser**:
   - The app will automatically open at `http://localhost:3000`
   - Or manually navigate to that URL

## API Key Configuration

⚠️ **Important**: You need to add your USDA FoodData Central API key to make the app work properly.

1. Get a free API key from: https://fdc.nal.usda.gov/api-key-signup.html

2. In `index.html`, find line 19 and replace `'DEMO_KEY'` with your actual API key:
   ```javascript
   const USDA_API_KEY = 'your-api-key-here'; // Replace with your actual USDA API key
   ```

**Note**: The DEMO_KEY has very limited requests. For regular use, you should get your own free API key.

## Usage

1. Click "Add Ingredient" to add ingredients manually
2. Enter the ingredient name, quantity, and select the unit
3. Set the number of servings
4. Click "Calculate Nutrition & Meal Pattern" to get results
5. View the nutrition facts and meal pattern crediting tables

## Supported Units

- oz (ounces)
- lbs (pounds)
- grams
- kg (kilograms)
- cups
- tbsp (tablespoons)
- tsp (teaspoons)
- ml (milliliters)
- l (liters)

## Technologies

- React 18
- Tailwind CSS
- Babel Standalone (for JSX transformation)
- USDA FoodData Central API
