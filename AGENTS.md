# Repository Guidelines

## Curate, Do Not Collect

Follow the [Awesome manifesto](https://github.com/sindresorhus/awesome/blob/main/awesome.md):
leave a candidate out when its value is uncertain. An entry must give ANTLR
users concrete value and be defensible through at least one of these: canonical
authority, demonstrated adoption and maintenance, foundational scholarship, or
a genuinely distinct capability. Popularity is supporting evidence, not proof.
Reject thin wrappers, generic parsing material that merely mentions ANTLR,
duplicative projects, SEO tutorials, and unverified self-promotion. When a
similar item exists, require a material difference.

## Place It Deliberately

- **Foundations:** primary papers and books explaining ANTLR or its algorithms.
- **The Tool:** the canonical generator and closely related ANTLR applications.
- **Runtime Targets:** code generators or runtimes for target languages.
- **Tooling:** editors, analysis, build, testing, visualization, and fuzzing.
- **Grammars:** collections; Vendor-Published only when the language or product
  owner publishes it, Community otherwise.
- **Benchmarks:** reproducible comparisons. **Learning:** durable documentation
  and substantive tutorials.

Do not create a category for one candidate. A new category should express a
durable distinction and have at least three credible entries. Preserve local
ordering; alphabetize only where the section already does so.

## Verify Before Writing

Search `README.md` for the name, owner, URL, and aliases. Open the resource and
inspect its documentation, releases, maintenance, and provenance. Prefer the
canonical HTTPS repository, specification, exact grammar path, or DOI. Verify
qualifiers such as "official," supported targets, maturity, and performance
against primary sources. Software should be maintained or demonstrably complete
and stable. Archived, experimental, or on-hold work needs exceptional value and
an explicit status note. Avoid volatile statistics in descriptions.

## Write and Submit

Use one unwrapped line:

```markdown
- [Canonical Name](https://canonical.example) - What it is and why it is distinct.
```

Use the project's exact styling. Keep the description objective, concise, and
punctuated; omit hype, "best," "leading," and unsupported claims. Link the
artifact itself, not a repost, search page, or tracking URL.

Make one resource the focus of each pull request. Update Contents only when
headings change, and avoid unrelated cleanup. In the PR, explain the user value,
verification evidence, and any affiliation. Use a specific title such as
`Add Foo to Tooling`. Before submission, open every changed link and run:

```sh
npx --yes awesome-lint
git diff --check
```

Repair moved canonical links first. Remove entries that are dead, misleading,
or superseded without enduring value.
