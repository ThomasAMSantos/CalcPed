# 🧙‍♂️ Grimório Pediátrico (CalcPed)

Uma ferramenta de bolso moderna, estilizada com a temática de **RPG e fantasia medieval**, criada para auxiliar magos curandeiros (médicos pediatras e clínicos gerais) no cálculo ágil de doses de medicamentos infantis.

O **Grimório Pediátrico** automatiza as regras matemáticas de prescrição com base no peso da criança, entregando as doses exatas, o formato da prescrição e gerando um **"Pergaminho de Cura"** (receituário) pronto para ser copiado para o prontuário.

-----

## ✨ Funcionalidades (Feitiços)

  * ⚖️ **Cálculo de Dose Baseado no Peso:** Insira o peso do paciente (em kg) e veja as doses (mL, gotas, jatos, comprimidos) serem calculadas instantaneamente.
  * 🗂️ **Catálogo Categorizado:** Medicamentos organizados logicamente (Antibióticos, Analgésicos, Anti-inflamatórios, Corticoides, Gastrointestinal, Hidratação, Respiratório, etc.).
  * 🔍 **Barra de Pesquisa Arcana:** Filtre poções ou ingredientes em tempo real pelo nome ou pela categoria.
  * 📜 **Geração de Pergaminho (Receita):** Selecione os medicamentos e clique em "Inscrever Pergaminho". O sistema gera um texto formatado com as posologias, pronto para copiar.
  * 🎇 **Efeitos Visuais Imersivos:** \* Rastro de poeira mágica que acompanha o cursor.
      * Explosões mágicas (*bursts*) ao selecionar (dourado) ou remover (cinza) itens do inventário.
  * 📱 **Design Responsivo:** Layout adaptável (Tailwind CSS) que funciona em desktops ou celulares, com menu lateral de scroll independente.

-----

## 🛠️ Tecnologias Utilizadas

Este artefato foi forjado utilizando tecnologias modernas em um único arquivo, dispensando servidores:

  * **HTML5:** Estrutura semântica.
  * **Tailwind CSS:** Estilização rápida e responsividade avançada via CDN.
  * **Vanilla JavaScript (ES6+):** Lógica matemática, filtros e manipulação de DOM.
  * **Font Awesome 6:** Iconografia temática.
  * **Google Fonts:** *Cinzel* para títulos arcanos e *Inter* para legibilidade clínica.

-----

## 🚀 Como Usar

O Grimório Pediátrico roda inteiramente no lado do cliente (*Client-side*), sem necessidade de Node.js ou bancos de dados.

1.  Faça o download do arquivo `index.html`.
2.  Abra o arquivo em qualquer navegador moderno (Chrome, Edge, Firefox, Safari).
3.  Insira o **Peso (kg)** no painel superior.
4.  Navegue pelas categorias ou pesquise o feitiço desejado.
5.  Marque o *checkbox* dos medicamentos que for utilizar.
6.  Clique em **"Inscrever Pergaminho"** na barra inferior dourada.
7.  Clique em **"Copiar Magia"** e cole no seu sistema de prontuário eletrônico (PEP).

-----

## ⚕️ Inclusão de Novos Medicamentos

Para adicionar novos feitiços, edite o array `medicamentos` dentro da tag `<script>` no final do arquivo HTML:

```javascript
{
    id: 'nome_unico_sem_espaco',
    categoria: 'Nome da Categoria',
    nome: 'Nome do Medicamento (Apresentação)',
    regraTexto: 'Descrição breve da dose mg/kg',
    baseCalculo: 'Ex: mg/kg/dose',
    calcular: (peso) => {
        // Lógica matemática
        let ml = peso * 0.5;
        return ml.toFixed(1); 
    },
    unidade: 'mL',
    posologia: 'Dar {dose} {unidade} por via oral, de X/X horas, por Y dias.'
}
```

-----

## ⚖️ Aviso Legal

Esta ferramenta tem como finalidade exclusiva auxiliar e agilizar a rotina de profissionais de saúde, **não substituindo o raciocínio clínico**. O criador não se responsabiliza por possíveis erros, omissões ou falhas nos cálculos.

**Cada usuário/profissional é inteiramente responsável** por conferir a exatidão dos dados (doses, concentrações e posologias) gerados antes de assinar ou anexá-los a qualquer prontuário oficial.

-----

## ✒️ Autor

Criado e idealizado por **Thomás Machado**.

  * 📸 **Instagram:** [@thomask\_machado](https://www.google.com/search?q=https://www.instagram.com/thomask_machado)
  * 📅 **Ano Estelar:** 2026