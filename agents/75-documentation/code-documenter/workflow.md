# Workflow

1. **Parse Files**: Read source files and extract function/class/module signatures
2. **Detect Format**: Identify existing doc format or use configured default
3. **Analyze Signatures**: Extract parameter names, types, default values, return types
4. **Generate Docs**: Create doc comments with @param, @returns, @throws tags
5. **Insert**: Place documentation comments before each declaration
6. **Preserve Existing**: Skip functions that already have complete docs
7. **Validate**: Check for syntax issues and format compliance
8. **Output**: Write updated source files with documentation
