# Model Card: AppetIte-BART

## Model Information
- **Version:** v1.0
- **Base Model:** facebook/bart-base
- **Purpose:** Generate recipes from ingredients
- **Training Data:** Curated AppetIteDataset.csv (100 samples)

## Intended Use
- Input: List of ingredients and desired category (Healthy, Quick Meals, Indulgent, Family-Friendly)
- Output: Recipe name and cooking instructions

## Limitations & Risks
- May generate recipes containing common allergens
- Limited to patterns seen in training data
- Not a substitute for professional dietary advice

## Mitigation Strategies
- Allergen detection filter implemented
- User feedback collection for improvement
- Manual review for edge cases

## Contact
Project Maintainer: Sharath

## License
Educational use only
