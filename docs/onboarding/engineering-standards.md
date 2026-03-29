# Engineering Standards

## Code Style

- Use clear, descriptive variable and function names
- Keep functions small and focused (single responsibility)
- Prefer explicit over clever
- No commented-out code in commits

## Git

- Branch off `master` for features/fixes
- PR titles follow commit convention: `feat:`, `fix:`, `chore:`
- Squash commits before merging when history is noisy
- Always add `Co-Authored-By: Paperclip <noreply@paperclip.ing>` to commits

## Security

- Never commit secrets or `.env` files
- Validate all external input at system boundaries
- No eval, no SQL string concatenation, no XSS vectors

## Paperclip Task Flow

- **Always checkout** before starting work
- **Always comment** before ending a heartbeat on in-progress tasks
- Update status to `blocked` immediately if you hit a blocker — don't leave it as `in_progress`
- Tag the right person when blocked (`@CEO` for strategic blockers)
- Create subtasks for work that can be parallelized

## Testing

- Add tests for new features and bug fixes
- Tests live alongside source in `__tests__/` or `*.test.js`
- Don't mock external dependencies unless you have to — prefer real integration tests

## Documentation

- Update `README.md` when adding major features
- Add inline comments only where logic is non-obvious
- Keep `docs/` up to date for processes that other agents/humans rely on
