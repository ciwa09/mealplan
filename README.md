# South India Meal Plan

A standalone South Indian family meal plan for Andhra Pradesh / Telangana style cooking. The app is built as a single HTML file and can be opened in a browser or shared as a static web page.

## File

- Main app: `india-meal-plan.html`

## What It Includes

- Month-length meal plan with breakfast, lunch, and dinner for 28, 29, 30, or 31 days.
- Adult portion target: under 1600 kcal per day.
- Family breakfast included for wife/kids, while the adult user can skip breakfast if desired.
- Vegetarian / Non-vegetarian selector.
- Vegetarian mode replaces non-veg meals with paneer, chana, rajma, or soya-based alternatives.
- Non-vegetarian mode schedules meat/fish lunches on actual Wednesdays and Sundays.
- Actual-calendar start date picker, defaulting to May 30, 2026.
- Weekly shopping lists.
- Recipe tab with ingredients, steps, helper notes, and concise cooking notes.
- Prep notes for helpers and family nutrition add-ons.
- No microwave or oven required.
- Designed around common South Indian ingredients.

## Nutrition Notes

The 1600 kcal number is an adult portion guide, not a restriction for kids.

For kids and active family members, add more food from the same meal base as needed:

- Extra idli, dosa, chapati, rice, or curd.
- One daily fruit such as banana, guava, orange, papaya, apple, pomegranate, or seasonal local fruit.
- 1 to 2 dairy servings such as milk, curd, buttermilk, or paneer.
- Small ghee serving where appropriate.
- Nuts or seeds if tolerated.

Use iodized salt. Vitamin D and B12 may still need sunlight, bloodwork, or doctor-guided supplementation, especially for fully vegetarian diets.

This meal plan is for general planning and convenience. It is not medical nutrition advice. For medical conditions, allergies, growth concerns, pregnancy, diabetes, kidney disease, anemia, or special pediatric needs, consult a doctor or registered dietitian.

## How To Open Locally

If you already have a local server running from the Downloads folder, open:

```text
http://localhost:8080/india-meal-plan.html
```

To start the local server from macOS Terminal:

```bash
cd ~/Downloads
python3 -m http.server 8080
```

Then open the same URL in a browser.

You can also double-click `india-meal-plan.html`, but using the local server is usually more reliable.

## Internet Requirement

The page uses CDN links for React, ReactDOM, Babel, and Google Fonts. The browser should have internet access when opening the page unless those dependencies are bundled later.

## Sharing Options

### Option 1: Send The File

Send `india-meal-plan.html` directly through email, chat, or cloud storage. Recipients can open it in a browser while online.

### Option 2: Netlify Drop

For a public link:

1. Create a folder.
2. Copy `india-meal-plan.html` into it.
3. Rename the copied file to `index.html`.
4. Go to `https://app.netlify.com/drop`.
5. Drag the folder into Netlify Drop.
6. Share the generated URL.

### Option 3: GitHub Pages

1. Create a GitHub repository.
2. Add the meal plan file as `index.html`.
3. Enable GitHub Pages in repository settings.
4. Share the generated GitHub Pages URL.

## How To Use The App

1. Choose `Vegetarian` or `Non-vegetarian` at the top.
2. Set the `Start date`; it defaults to May 30, 2026 and remembers changes in the same browser.
3. Use the day buttons to move through the selected month length; each day shows the actual weekday and date.
4. Open the `Plan` tab for daily meals and macros.
5. Open the `Recipes` tab for cooking steps.
6. Open the `Prep` tab for batching and family nutrition notes.
7. Open the `Ingredients` tab for weekly shopping lists.
8. Check off ingredients as you shop.

## Cooking Setup

Useful kitchen tools:

- Pressure cooker.
- Kadai.
- Tawa.
- Idli steamer.
- Mixer jar.
- Rice cooker, optional.
- Measuring cups and spoons.

No microwave or oven is needed.

## Maintenance Notes

The app is a single-file React app using Babel in the browser. All data, styles, and components are inside `india-meal-plan.html`.

When editing:

- Keep daily adult totals under 1600 kcal unless intentionally changing the target.
- Update both normal and vegetarian replacement meals if changing Wednesday/Sunday non-veg templates.
- Update weekly shopping lists when adding new recurring ingredients.
- Keep recipe steps practical for home cooks and helpers.
- Recheck the page in a browser after edits because one JSX syntax error can blank the page.

## Current Validation

The current version was checked for:

- 28, 29, 30, and 31-day month lengths.
- Actual calendar dates from the selected start date.
- Wednesday/Sunday non-veg scheduling.
- Vegetarian replacement logic.
- Weekly shopping lists.
- Adult daily calorie totals under 1600 in both diet modes.
- Family nutrition add-ons.
- Recipe cooking notes.
- Local serving through `http://localhost:8080/india-meal-plan.html`.
