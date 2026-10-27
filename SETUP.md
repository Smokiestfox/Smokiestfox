# Profile setup

1. Create a **public** GitHub repository named **Smokiestfox** under the Smokiestfox account.
2. Upload `README.md`, the complete `assets` directory, and `.github/workflows/snake.yml` to its root.
3. Commit the files. GitHub will display this README on the profile.

The banner, typing greeting, and footer are self-contained animated SVGs. The tool icons are loaded from [Skill Icons](https://github.com/tandpfun/skill-icons).

The contribution snake is generated from Smokiestfox's contribution calendar with [Platane/snk](https://github.com/Platane/snk). The `Update contribution snake` GitHub Actions workflow runs daily at approximately 07:17 Bangkok time and can also be run manually. It publishes matching light and dark SVGs to the `output` branch using GitHub's built-in workflow token. No personal token needs to be added.

The README uses English for a broad audience. Its introduction says:

> Tôi đang định hướng trở thành Backend Developer. Tôi thích khám phá các ý tưởng thực tế và biến chúng thành phần mềm hữu ích.

Suggested GitHub bio:

```text
Aspiring Backend Developer · Exploring practical ideas · Java, TypeScript & Python
```

## Maintaining the profile

| File | Purpose |
| --- | --- |
| `README.md` | Introduction, tools, contact, and image references |
| `assets/header.svg` | Animated fox terminal banner |
| `assets/intro.svg` | Alternating typing greeting |
| `assets/footer.svg` | Animated divider |
| `.github/workflows/snake.yml` | Generates and publishes the contribution snakes |

Edit the introduction, tool list, or contact address in `README.md`. The custom SVGs contain their own text, colors, and animation timings; they can be edited directly without a build step. When changing a typing message, also adjust its text length, reveal width, and cursor travel so they stay aligned.

Open the individual SVG files in a browser to check the animations, then check the README on GitHub for its final spacing. Reduced-motion preferences disable the custom banner, greeting, and footer animations in supporting browsers.

### Refreshing the contribution snake

1. Open this repository's **Actions** tab.
2. Select **Update contribution snake** and choose **Run workflow** on `main`.
3. Wait for the run to succeed, then check `github-snake.svg` and `github-snake-dark.svg` on the `output` branch.

The workflow generates both files from this account's real contribution calendar. Change the palette in the workflow to customize their colors. Edit the workflow rather than the generated files on `output`, since the next run replaces those files.

If a snake image is missing, inspect the latest workflow run before changing its README URL. Scheduled runs may start later than their configured time; **Run workflow** provides a manual refresh.

## Inspiration

- [DenverCoder1/readme-typing-svg](https://github.com/DenverCoder1/readme-typing-svg): animated typing.
- [Platane](https://github.com/Platane) and [Platane/snk](https://github.com/Platane/snk): contribution-snake animation.
- [AVIVASHISHTA29](https://github.com/AVIVASHISHTA29): terminal-inspired profile composition.
- [Anmol-Baranwal](https://github.com/Anmol-Baranwal): concise, personal introduction and contact placement.
- [phamhuulocforwork](https://github.com/phamhuulocforwork): a separate typing greeting and contribution-snake section; the existing fox banner is retained.

The custom fox, banner, and footer were drawn specifically for this profile. No artwork was copied from the reference profiles.
