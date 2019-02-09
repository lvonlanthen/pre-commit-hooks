# pre-commit hooks

Some custom pre-commit hooks for [pre-commit](https://github.com/pre-commit/pre-commit).

### Using pre-commit-hooks with pre-commit

Add this to your `.pre-commit-config.yaml`

    -   repo: https://github.com/lvonlanthen/pre-commit-hooks
        rev: v1.0.0  # Use the ref you want to point at
        hooks:
        -   id: js-debug-statements
        # -   id: ...

### Hooks

- `js-debug-statements` - Check Vue (`.vue`) and JavaScript files for debug statements, such as:
    - `console.log`
    - `debugger`
    
- `py-check-pytest-marks` - Check Python files for pytest marks used for local development, such as:
    - `@pytest.mark.foo` 
    - `@pytest.mark.bar`
