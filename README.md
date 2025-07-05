d# Controle-de-ragas
git init
git remote add origin https://github.com/SEU_USUARIO/controle-pragas-sincop.git
# Adicione os arquivos baixados manualmente no diretório
git add .
git commit -m "Versão inicial do site React com Firebase"
git push -u origin master
controle-pragas-sincop/
├── public/
│   └── index.html
├── src/
│   ├── App.jsx
│   ├── firebaseConfig.js
│   └── index.js
├── package.json
├── tailwind.config.js
├── postcss.config.js
├── .gitignore
└── README.md
cd functions
npm install
firebase deploy --only functions
