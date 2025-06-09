from pathlib import Path
from markdown2 import markdown

# Conteúdo formatado para o Notion mobile-friendly com caixas de seleção
roteiro_markdown = """
# 📝 ROTEIRO DE ANAMNESE OFTALMOLÓGICA
### 📍 Consulta prática, clínica popular

---

## 👤 1. DADOS INICIAIS
- [ ] Nome completo
- [ ] Idade
- [ ] Profissão
- [ ] Lateralidade (OD / OE / ambos)
- [ ] Queixa principal: _"O que está te incomodando hoje nos olhos?"_

---

## ⏳ 2. INÍCIO E DURAÇÃO DOS SINTOMAS
- [ ] Quando começou?
- [ ] Está piorando, melhorando ou igual?
- [ ] É contínuo ou vem e vai?

---

## 🔍 3. SINTOMAS OCULARES
Marcar os positivos:
- [ ] Ardência
- [ ] Olho vermelho
- [ ] Secreção (aguada, amarelada?)
- [ ] Dor nos olhos
- [ ] Sensação de areia ou corpo estranho
- [ ] Fotofobia
- [ ] Coceira
- [ ] Lacrimejamento
- [ ] Piora ao computador ou leitura
- [ ] Visão embaçada

---

## 👓 4. USO DE ÓCULOS / LENTES
- [ ] Usa óculos? (longe, perto, ambos?)
- [ ] Troca recente do grau?
- [ ] Usa lentes de contato? Tipo? Frequência?

---

## 🧴 5. MEDICAÇÕES USADAS
- [ ] Está usando algum colírio? Qual?
- [ ] Já tratou isso antes?

---

## 🧬 6. ANTECEDENTES OFTALMOLÓGICOS
- [ ] Problemas anteriores nos olhos
- [ ] Cirurgia ocular? Trauma? Infecção?
- [ ] Histórico familiar (glaucoma, degeneração, cegueira)

---

## 🩺 7. DOENÇAS SISTÊMICAS
- [ ] Hipertensão
- [ ] Diabetes
- [ ] Medicamentos contínuos

---

## 🔔 8. SINAIS DE ALERTA
- [ ] Dor ocular intensa com náusea?
- [ ] Visão com halos ou perda súbita?
- [ ] Trauma ocular recente?
- [ ] Uso recente de lentes de contato?

---

## 📌 9. FINALIZAÇÃO
- [ ] Algo mais que te incomoda nos olhos?
- [ ] Deseja fazer algum exame?

---

## 🧠 DICA DO MENTOR
💡 Sempre classifique:
- [ ] Lateralidade (uni/bilateral)
- [ ] Intensidade (leve/moderada/intensa)
- [ ] Tipo de secreção (aquosa/mucosa/purulenta)
- [ ] Tempo de evolução (<1 sem / semanas / meses)
"""

# Salvar o conteúdo como arquivo Markdown
output_path = Path("/mnt/data/Roteiro_Anamnese_Oftalmologica_Notion.md")
output_path.write_text(roteiro_markdown.strip())

output_path.name
# html
