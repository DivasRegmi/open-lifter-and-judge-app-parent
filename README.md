# open-lifter-and-judge-app-parent

Parent repository combining related projects as git submodules.

## Projects

| Directory | Repository | Description |
|-----------|-----------|-------------|
| `judge-app/` | [DivasRegmi/judge-app](https://github.com/DivasRegmi/judge-app) | Expo/React Native app |
| `open-lifter/` | [DivasRegmi/open-lifter](https://github.com/DivasRegmi/open-lifter) | Tauri + web app |
| `backend/` | [DivasRegmi/byayam-backend](https://github.com/DivasRegmi/byayam-backend) | Java/Spring Boot backend |

## Cloning

Clone with all submodules in one command:

```bash
git clone --recurse-submodules git@github.com:DivasRegmi/open-lifter-and-judge-app-parent.git
```

If you already cloned without `--recurse-submodules`:

```bash
git submodule update --init --recursive
```

## Updating Submodules

To pull latest changes for all submodules:

```bash
git submodule update --remote --merge
```

To update a specific submodule:

```bash
cd judge-app
git pull origin main
cd ..
git add judge-app
git commit -m "Update judge-app submodule"
```
