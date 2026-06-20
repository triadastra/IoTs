# Contributing to IoTs Index

Thank you for your interest in contributing to the IoT Index project! This document provides guidelines for making contributions that maintain quality and consistency across the repository.

## Ways to Contribute

1. **New Topic Documents** — Add documentation on IoT technologies, protocols, or trends
2. **Improvements** — Enhance existing documentation with more detail or examples
3. **Citations & References** — Add academic sources and industry insights
4. **Corrections** — Fix errors or outdated information
5. **Feedback** — Report issues or suggest improvements

## Getting Started

### 1. Fork and Clone
```bash
git clone <repository-url>
cd IoTs
git checkout -b feature/your-topic-name
```

### 2. Choose a Topic Category

Select the appropriate directory:
- `docs/protocols/` — Communication protocols
- `docs/applications/` — Real-world IoT applications
- `docs/security/` — Security and privacy topics
- `docs/architecture/` — System design and infrastructure
- `docs/trends/` — Emerging technologies and future directions

### 3. Use the Document Template

Copy the template and follow its structure:
```bash
cp docs/TEMPLATE.md docs/your-category/your-topic.md
```

## Document Guidelines

### Structure

Every document should follow this structure:

1. **Title** (`# Topic Name`)
2. **Overview** — What is this? Why does it matter?
3. **Key Concepts** — Essential terminology and ideas
4. **Current Status** — State as of 2026
5. **Use Cases / Applications** — Real-world examples
6. **Architecture / Examples** — Diagrams or illustrations
7. **References & Citations** — Academic and industry sources
8. **Related Topics** — Links to connected documents
9. **Metadata** — Version, date, contributors

### Style Guidelines

- **Tone** — Professional, accessible to non-experts
- **Length** — 1,500-3,000 words for depth without overwhelming
- **Code Examples** — Use fenced code blocks with language identifiers
- **Headings** — Use ATX-style (`#`, `##`, `###`)
- **Links** — Use relative paths for internal links: `[Topic](./filename.md)`
- **Line Length** — Keep prose to 80-120 characters per line

### Citation Format

Include both inline citations and a References section:

```markdown
## References & Citations

1. Author Name (Year). "Article/Book Title" — Publication/Publisher
2. [Online Resource Name](https://example.com/) — Description
```

### Example Citation Types

**Academic Paper:**
```
Smith, J. & Doe, A. (2025). "IoT Protocol Analysis" — IEEE Transactions on IoT
```

**Book:**
```
Johnson, M. (2024). "Internet of Things Fundamentals" — O'Reilly Media
```

**Website/Blog:**
```
[AWS IoT Documentation](https://docs.aws.amazon.com/iot/) — Official guides and references
```

## Before Submitting

### Quality Checklist

- [ ] Document follows the template structure
- [ ] Content is accurate and current (2026 perspective)
- [ ] At least 3-5 citations/references included
- [ ] Internal links to related topics are added
- [ ] Links are tested and working
- [ ] No spelling or grammar errors
- [ ] Code examples (if any) are correct
- [ ] Metadata section is complete

### Testing Links

Verify all links work before submission:
```bash
# Check relative links manually
# Ensure external links resolve to valid pages
```

## Pull Request Process

1. **Create a descriptive branch name**
   ```bash
   git checkout -b feature/mqtt-security-update
   git checkout -b docs/edge-computing-expansion
   ```

2. **Make your changes** and commit with clear messages
   ```bash
   git commit -m "Add documentation on MQTT security best practices"
   ```

3. **Update the main README** if adding a new major topic
   - Add entry to navigation section
   - Update relevant category sections

4. **Push to your fork** and create a pull request
   ```bash
   git push origin feature/your-topic-name
   ```

5. **PR Description** should include:
   - What you added/changed
   - Why it's important
   - Any new references or sources
   - Related issues (if applicable)

## Maintainer Review Process

Submissions will be reviewed for:
- **Accuracy** — Factually correct information
- **Relevance** — Aligned with IoT focus
- **Quality** — Well-written and well-organized
- **Citations** — Proper attribution of sources
- **Consistency** — Matches project style and structure

Reviewers will provide feedback within 1-2 weeks.

## Content Standards

### Accuracy & Timeliness
- Content should reflect the 2026 landscape
- Include recent data and trends
- Cite sources dated 2024 or later where possible
- Clearly mark outdated information as historical

### Neutrality
- Avoid promotional content for specific vendors
- Represent multiple perspectives fairly
- Disclose any conflicts of interest
- Focus on technical merit, not marketing

### Completeness
- Cover both advantages and limitations
- Address security and privacy implications
- Include practical considerations
- Suggest when to use vs. not use a technology

## Questions or Need Help?

- Open an issue with questions or suggestions
- Check existing documents for structure examples
- Review past PRs to see accepted styles
- Contact maintainers for guidance

## License

By contributing, you agree that your work will be licensed under the repository's license (to be specified).

---

**Last Updated:** 2026-03-04
**Thank you for contributing to the IoT Index!**
