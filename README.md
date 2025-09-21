gbraad's Dotfiles `action` Actionfile executor
==============================================

Runs `action` from my dotfiles to run [Actionfiles](https://github.com/actionfile), a Markdown-based configuration file that describes a set of actions, scripts, or tasks for use in automation workflows

### Usage

```yaml
      - name: Setup environment
        uses: gbraad-dotfiles/install-action@main

      ... checkout code ...

      - name: Use actionfile to compile crc
        uses: gbraad-dotfiles/actionfile-action@main
        with:
          file: ./crc.md
          action: compile devenv
```
