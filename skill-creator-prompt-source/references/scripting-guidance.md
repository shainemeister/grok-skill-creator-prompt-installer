# Scripting Recommendations

Recommend adding Python (or other) scripts in `scripts/` when the skill needs:

- Deterministic and repeatable operations (validation, formatting, calculations, data transformation)
- File processing or structured data handling
- Better long-term testability and maintainability
- Complex logic that is clearer in code than in prompt instructions

**Best Practice**:
- Keep high-level reasoning, planning, and user interaction in the `SKILL.md` prompt.
- Move well-defined, repeatable work to scripts.

This hybrid approach produces more reliable and maintainable skills.