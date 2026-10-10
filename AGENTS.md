<!-- LOVABLE:BEGIN -->
> [!IMPORTANT]
> This project is connected to [Lovable](https://lovable.dev). Avoid rewriting
> published git history — force pushing, or rebasing/amending/squashing commits
> that are already pushed — as it rewrites history on Lovable's side and the
> user will likely lose their project history.
>
> Commits you push to the connected branch sync back to Lovable and show up in
> the editor, so keep the branch in a working state.
<!-- LOVABLE:END -->

## Architecture
- Keep the book catalog as a curated browser-safe module and store member reading records in Cloud with owner-only RLS, so public browsing remains independent of authentication.
- Use one root member provider for session changes and a client-only authenticated route layout for member pages, because account sessions are browser-managed.
- Use the shared library shell and CSS semantic tokens for all content routes, so navigation and presentation remain consistent.
