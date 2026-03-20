🧙‍♂️ Grimório Pediátrico (CalcPed)

Uma ferramenta de bolso moderna, estilizada com a temática de RPG e fantasia medieval, criada para auxiliar magos curandeiros (médicos pediatras e clínicos gerais) no cálculo ágil de doses de medicamentos infantis.

O Grimório Pediátrico automatiza as regras matemáticas de prescrição com base no peso da criança, entregando as doses exatas, formato da prescrição e até mesmo gerando um "Pergaminho de Cura" (receituário) pronto para ser copiado para o prontuário.

✨ Funcionalidades (Feitiços)

⚖️ Cálculo de Dose Baseado no Peso: Insira o peso do paciente (em kg) e veja as doses (mL, gotas, jatos, comprimidos) serem calculadas instantaneamente.

🗂️ Catálogo Categorizado: Medicamentos organizados logicamente (Antibióticos, Analgésicos, Anti-inflamatórios, Corticoides, Gastrointestinal, Hidratação Venosa/Oral, Respiratório, etc.).

🔍 Barra de Pesquisa Arcana: Filtre poções ou ingredientes em tempo real pelo nome ou pela categoria.

📜 Geração de Pergaminho (Receita): Selecione os medicamentos que deseja prescrever e clique em "Inscrever Pergaminho". O sistema gera um texto formatado com as posologias, pronto para copiar com um clique.

🎇 Efeitos Visuais Imersivos: * Rastro de poeira mágica que acompanha o cursor do mouse.

Explosões mágicas (bursts) ao selecionar (dourado) ou remover (cinza) um medicamento do seu inventário.

📱 Design Responsivo: Layout adaptável (usando Tailwind) que funciona perfeitamente em telas imensas ou na palma da sua mão através do celular. Aba de menu lateral com scroll independente para não perder o foco da tela.

🛠️ Tecnologias Utilizadas

Este artefato foi forjado utilizando tecnologias modernas e ágeis em um único arquivo, dispensando servidores ou instalações complexas:

HTML5 para a estrutura semântica.

Tailwind CSS (via CDN) para a estilização rápida e responsividade avançada.

Vanilla JavaScript (ES6+) para toda a lógica matemática, filtros e manipulação de estado (DOM).

Font Awesome 6 para a iconografia temática.

Google Fonts (Cinzel para os títulos arcanos e Inter para legibilidade de dados clínicos).

🚀 Como Usar

O Grimório Pediátrico não requer instalação de pacotes (Node.js, npm, etc.) ou bancos de dados externos. Ele roda inteiramente no lado do cliente (Client-side).

Faça o download do arquivo index.html.

Dê um duplo clique no arquivo para abri-lo em qualquer navegador moderno (Chrome, Edge, Firefox, Safari).

Insira o Peso (kg) no painel superior.

Navegue pelas categorias laterais ou pesquise o feitiço desejado.

Marque o checkbox dos medicamentos que for utilizar.

Clique em "Inscrever Pergaminho" na barra inferior dourada.

Clique em "Copiar Magia" e cole no seu sistema de prontuário eletrônico (PEP).

⚕️ Inclusão de Novos Medicamentos

Para adicionar novos "feitiços" ao grimório, basta editar o array medicamentos dentro da tag <script> no final do arquivo HTML.

A estrutura de um novo medicamento é a seguinte:

{
    id: 'nome_unico_sem_espaco',
    categoria: 'Nome da Categoria',
    nome: 'Nome do Medicamento (Apresentação)',
    regraTexto: 'Descrição breve da dose mg/kg',
    baseCalculo: 'Ex: mg/kg/dose',
    calcular: (peso) => {
        // Lógica matemática para calcular o resultado
        let ml = peso * 0.5;
        return ml.toFixed(1); // Retorne como string para padronizar casas decimais
    },
    unidade: 'mL',
    posologia: 'Dar {dose} {unidade} por via oral, de X/X horas, por Y dias.'
}


O sistema automaticamente reconhecerá a nova categoria (se for inédita), criará a seção e fará o binding dos cálculos sem necessidade de mexer em HTML ou CSS.

⚖️ Aviso Legal

Esta ferramenta tem como finalidade exclusiva auxiliar e agilizar a rotina de profissionais de saúde, não substituindo o raciocínio clínico e o bom senso. O criador não se responsabiliza por possíveis erros, omissões ou falhas nos cálculos decorrentes do uso da aplicação.

Cada usuário/profissional é inteiramente responsável por conferir a exatidão dos dados (doses, concentrações e posologias) gerados antes de assinar, prescrever ou anexá-los a qualquer prontuário oficial.

✒️ Autor

Criado e idealizado por Thomás Machado.

Instagram: @thomask_machado

Ano Estelar: 2026