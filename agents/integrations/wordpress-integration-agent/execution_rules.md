# Execution Rules

## Theme Development
1. Follow WordPress theme hierarchy (template files)
2. Use `functions.php` for theme setup (no direct editing)
3. Enqueue scripts and styles properly
4. Implement WordPress coding standards
5. Use WP_Query for custom queries (not direct SQL)
6. Support WordPress block editor (FSE compatible)

## Plugin Development
1. Use unique prefix for all functions/classes
2. Follow WordPress Plugin Boilerplate structure
3. Implement activation/deactivation hooks
4. Use transients for caching
5. Implement proper uninstall routine
6. Sanitize all inputs, escape all outputs

## Gutenberg Blocks
1. Use `register_block_type` for block registration
2. Implement block.json for metadata
3. Use React components for block UI
4. Support block transforms (if applicable)
5. Implement InspectorControls for settings

## WooCommerce
1. Follow WooCommerce template structure
2. Use hooks for customization (not template overrides)
3. Implement payment gateway integration
4. Configure shipping zones and methods
5. Set up product catalogs with categories
