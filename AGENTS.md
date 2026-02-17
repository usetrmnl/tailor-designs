# Tailor Designs Repository

## Purpose
This repository stores screen designs created by individuals. Screens are pushed via pull requests and validated through a GitHub Actions workflow.

## File Structure
- `screens/` - Directory containing all screen files
- `.github/workflows/validate-images.yml` - Workflow that validates file naming conventions

## Naming Convention
Files in the `screens/` directory must follow this format:
```
{WIDTH}x{HEIGHT}-{TYPE}-{NAME}.{EXT}
```

Where:
- `{WIDTH}x{HEIGHT}` - Screen resolution (e.g., 800x480)
- `{TYPE}` - Type of screen, either "loading" or "splash"
- `{NAME}` - Descriptive name using lowercase letters, numbers, underscores
- `{EXT}` - File extension (must be PNG)

## Example Files
- `800x480-splash-hourglass_with_butterflies.png`
- `800x480-loading-dungeon_crawler_carl_princess_donut.png`

## Gallery Features
The gallery webpage provides:
- Filter by screen type (splash/loading)
- Search functionality
- Responsive grid layout
- Modern UI with Tailwind CSS styling

## Validation Workflow
The validation workflow ensures all files:
1. Use only lowercase letters, numbers, underscores, and hyphens
2. Have 3 or 4 segments separated by hyphens
3. Have a valid PNG file format
4. Match the specified dimensions in filename with actual image dimensions
5. Have the correct type (loading or splash)