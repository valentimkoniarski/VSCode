# VSCode
Configurações do VSCode


No **VSCode** devem ser instaladas as seguintes extensões:
> **Obrigatórias**
> - [EditorConfig for VS Code](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig)
> - [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
> - [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)

> **Recomendadas**
> - [Auto Close Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-close-tag)
> - [vscode-js-import](https://marketplace.visualstudio.com/items?itemName=wangtao0101.vscode-js-import)
> - [Auto Rename Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag)
> - [GitLens — Git supercharged](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
> - [npm](https://marketplace.visualstudio.com/items?itemName=eg2.vscode-npm-script)
> - [npm Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.npm-intellisense)
> - [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
> - [Project Manager](https://marketplace.visualstudio.com/items?itemName=alefragnani.project-manager)
> - [vscode-icons](https://marketplace.visualstudio.com/items?itemName=robertohuertasm.vscode-icons)


Após a instalação das extensões obrigatórias, deve ser adicionadas as seguintes configurações na pasta .vscode/arquivo.json:

**>Preferences: Open Settings (JSON)**

> - "javascript.format.enable": false
> - "eslint.validate": ["javascript"]
> - "prettier.eslintIntegration": true

## Instalação

Para baixar as dependências do projeto (construção e view), execute o comando:

```
npm install
```


## Execução

O projeto usa o webpack para a construção.
Para construir e executar o aplicativo, execute o comando:

```
npm start
```


Para configurar o vscode settings.json
```
{
  "git.enableSmartCommit": true,
  "git.autofetch": true,
  "git-autoconfig.configList": [
    {
      "user.email": "valentim.koniarski@hotmail.com",
      "user.name": "valentimkoniarski"
    }
  ],
  "workbench.iconTheme": "vscode-icons",
  "editor.formatOnSave": true,
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "[javascript]": {
    "editor.formatOnSave": false
  },
  "[vue]": {
    "editor.formatOnSave": true
  },
  "editor.codeActionsOnSave": {
    "source.fixAll": true,
    "source.fixAll.eslint": true
  },

  "eslint.format.enable": true,
  "javascript.updateImportsOnFileMove.enabled": "always"
}
```

