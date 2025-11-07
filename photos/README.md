# Photos & Documentation

Store photos, diagrams, and other documentation for Gemma's restoration.

## Organization

Organize photos by category or date:

```
photos/
├── before/           # Initial condition photos
├── progress/         # Work-in-progress photos
├── after/            # Completed work photos
├── parts/            # Photos of parts before/after
├── reference/        # Reference materials, diagrams, manuals
└── YYYY-MM-DD/      # Date-based folders for work sessions
```

## Naming Convention

Use descriptive names for photos:
- `2025-01-15-engine-bay-before.jpg`
- `2025-02-10-passenger-door-rust.jpg`
- `2025-03-05-brake-caliper-rebuilt.jpg`

## Referencing Photos

Link photos from work logs using relative paths:
```markdown
![Description](../photos/2025-01-15-engine-bay-before.jpg)
```
