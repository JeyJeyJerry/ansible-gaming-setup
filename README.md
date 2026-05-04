# Ansible Gaming Setup

Palvelinten hallinta-kurssin projekti peliympäristön automatisointiin

## Mihin tarkoitukseen?

- Päivittää käyttöjärjestelmän
- Varmistaa, että uusimmat NVIDIA-ajurit ovat asennettu
- Aentaa `Discordin` ja `Steamin` 

## Käyttöohjeet

- **Playbookin** toimimista varten täytyy olla paketit `ansible`, `git` ja `openssh-server` asennettuna
- Ansiblen ja git saa asennettua komenolla:

```bash
sudo apt install ansible git openssh-server
```

- Käynnistä **SSH-demoni** ja varmista, että se toimii komennoilla:

```bash
sudo systemctl enable --now ssh
sudo systemctl status ssh
```

- Kun demoni on päällä varmista vielä, että yhteys toimii komennolla:

```bash
ssh localhost
```

- Tämän jälkeen kopioi varasto komennolla:

```bash
git clone https://github.com/JeyJeyJerry/ansible-gaming-setup.git
```

- Aja kopioidun kansion sisällä komento:

```bash
ansible-playbook site.yml
```

- Terminaalissa näkyy vaiheittain, mitä ohjelma tekee
- Latauksen päätyttyä koneellasi on asennettuna **Discord** ja **Steam** valmiina pelaamiseen
