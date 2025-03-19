# To get dependencies
```
conda env create -f environment.yml
```

# Dataset
Source: [kaggle](https://www.kaggle.com/datasets/nadyinky/sephora-products-and-skincare-reviews)

Move the csv files into `data` folder

# Feature Descriptions for Sephora Dataset
## Product Details
- product_id – Unique identifier for the product from the site.
- product_name – Full name of the product.
- brand_id – Unique identifier for the product brand from the site.
- brand_name – Full name of the product brand.

## Popularity & User Engagement
- loves_count – Number of people who have marked this product as a favorite.
- rating – Average rating of the product based on user reviews.
- reviews – Number of user reviews for the product.

## Product Variations
- size – Size of the product (e.g., oz, ml, g, packs, etc.).
- variation_type – Type of variation parameter (e.g., Size, Color).
- variation_value – Specific value of the variation parameter (e.g., 100 mL, Golden Sand).
- variation_desc – Description of the variation parameter (e.g., "tone for fairest skin").

## Composition & Ingredients
- ingredients – List of ingredients included in the product. Example formats:
    - [‘Product variation 1:’, ‘Water, Glycerin’]
    - [‘Product variation 2:’, ‘Talc, Mica’]
    - [‘Water, Glycerin’] (if no variations)

## Pricing Details
- price_usd – Regular price of the product in US dollars.
- value_price_usd – Potential cost savings, presented on the site next to the regular price.
- sale_price_usd – Sale price of the product in US dollars.

## Product Availability & Exclusivity
- limited_edition – Indicates if the product is a limited edition (1 = true, 0 = false).
- new – Indicates if the product is new (1 = true, 0 = false).
- online_only – Indicates if the product is sold exclusively online (1 = true, 0 = false).
- out_of_stock – Indicates if the product is currently out of stock (1 = true, 0 = false).
- sephora_exclusive – Indicates if the product is exclusive to Sephora (1 = true, 0 = false).

## Product Highlights & Categories
- highlights – List of tags or features that highlight the product's attributes (e.g., [‘Vegan’, ‘Matte Finish’]).
- primary_category – First category in the breadcrumb section.
- secondary_category – Second category in the breadcrumb section.
- tertiary_category – Third category in the breadcrumb section.

## Product Variants & Price Range
- child_count – Number of variations available for the product.
- child_max_price – Highest price among the variations.
- child_min_price – Lowest price among the variations.