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
/tecnicos
  └── {tecnicoId}
       └── nome: "João Silva"
       └── cpf: "123.456.789-00"
       └── pin: "1234"
       └── email: "joao@empresa.com"

/ordens_servico
  └── {osId}
       └── tecnicoId: "tecnico123"
       └── cliente: {
              nome: "Maria Souza",
              endereco: "Rua das Flores, 123"
          }
       └── tipoPraga: "Baratas"
       └── ambiente: "Cozinha"
       └── produto: {
              nome: "Inseticida X",
              lote: "L12345",
              validade: "2025-10"
          }
       └── dosagem: "10ml/m²"
       └── epIs: "Luvas, Máscara"
       └── responsavelTecnico: "Eng. Marcos (CRQ 12345)"
       └── inicio: Timestamp
       └── fim: Timestamp
       └── localizacao: GeoPoint
       └── assinaturaTecnico: "base64"
       └── assinaturaCliente: "base64"
       └── pdfLaudoUrl: "https://..." (gerado após conclusão)
