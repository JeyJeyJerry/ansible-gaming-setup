# Ansible Gaming Setup

Palvelinten hallinta-kurssin projekti peliympäristön automatisointiin

## Mihin tarkoitukseen?

- Päivittää käyttöjärjestelmän
- Varmistaa, että uusimmat NVIDIA-ajurit ovat asennettu
- Aentaa `Discordin` ja `Steamin` 

## Käyttöohjeet

- **Playbookin** toimimista varten täytyy olla paketit `ansible` ja `git` asennettuna
- Ansiblen ja git saa asennettua komenolla:

````
$ sudo apt install ansible git
````

- Tämän jälkeen kopioi varasto komennolla: `git clone https://github.com/JeyJeyJerry/ansible-gaming-setup.git`
- Aja kopioidun kansion sisällä komento `ansible-playbook site.yml`
  - Terminaalissa näkyy vaiheittain, mitä ohjelma tekee
  - Latauksen päätyttyä koneellasi on asennettuna **Discord** ja **Steam** valmiina pelaamiseen
