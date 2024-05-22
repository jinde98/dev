# GitHub Dev Container with Chromium

This project provides a `docker-compose.yml` file to set up a Chromium browser in a GitHub Dev Container. This can be particularly useful for accessing websites with IP restrictions.

# GitHub Dev 容器中的 Chromium

本项目提供了一个 `docker-compose.yml` 文件，用于在 GitHub Dev 容器中设置 Chromium 浏览器。这对于访问有 IP 限制的网站特别有用。

## Usage

### 使用方法

1. **Create a Dev Container**:
   - Initialize a Dev Container for your project by creating a `.devcontainer` folder with a `devcontainer.json` file in the root of your repository. You can use the [GitHub Super Linter](https://github.com/github/super-linter) as a template.

   **创建 Dev 容器**：
   - 通过在项目的根目录创建一个带有 `devcontainer.json` 文件的 `.devcontainer` 文件夹，为你的项目初始化一个 Dev 容器。你可以使用 [GitHub Super Linter](https://github.com/github/super-linter) 作为模板。

2. **Add the `docker-compose.yml` File**:
   - Place the provided `docker-compose.yml` file in the `.devcontainer` folder.

   **添加 `docker-compose.yml` 文件**：
   - 将提供的 `docker-compose.yml` 文件放入 `.devcontainer` 文件夹中。

3. **Open the Project in GitHub Codespace**:
   - Open your repository in a GitHub Codespace by going to your repository's page on GitHub and clicking on the "Code" tab, then "Open codespace for this repository".

   **在 GitHub Codespace 中打开项目**：
   - 通过访问你的 GitHub 仓库页面，点击 "Code" 标签，然后选择 "Open codespace for this repository" 在 GitHub Codespace 中打开你的仓库。

4. **Start the Chromium Container**:
   - Once the Codespace is ready, open a new terminal and run the following command to start the Chromium container:

   **启动 Chromium 容器**：
   - Codespace 准备就绪后，打开一个新的终端并运行以下命令以启动 Chromium 容器：

     ```bash
     docker-compose up -d
     ```

   - This will start the Chromium container in detached mode.

   - 这将以分离模式启动 Chromium 容器。

5. **Access the Chromium Instance**:
   - You can now access the Chromium instance through the specified ports (default: `3000` for Chromium and `3001` for the HTTP/WS proxy).

   **访问 Chromium 实例**：
   - 你现在可以通过指定的端口（默认：`3000` 用于 Chromium，`3001` 用于 HTTP/WS 代理）访问 Chromium 实例。

## Support

For support or issues, consider opening a ticket in this repository or joining the LinuxServer.io community on [Discord](https://discord.gg/YWrKVTn) or [Discourse](https://discourse.linuxserver.io/).

## 支持

如需支持或遇到问题，请考虑在此仓库中提出问题或加入 LinuxServer.io 社区的 [Discord](https://discord.gg/YWrKVTn) 或 [Discourse](https://discourse.linuxserver.io/)。

