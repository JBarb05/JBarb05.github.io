---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2026-01-05
type: landing

design:
  # Default section spacing
  spacing: '0'

sections:
  # Hero développeur - Fond dégradé avec nom, rôle, réseaux sociaux et CTA
    - block: dev-hero
      id: hero
      content:
        username: me
        greeting: "Bonjour, je suis"
        show_status: true
        show_scroll_indicator: true
        typewriter:
          enable: true
          prefix: "Je travaille sur"
          strings:
            - "des systèmes spécifiques"
            - "de la VoIP"
            - "de la pose de cable"
            - "des outils open source"
          type_speed: 70
          delete_speed: 40
          pause_time: 2500
        cta_buttons:
          - text: Mes projets
            url: "#projects"
            icon: arrow-down
          - text: Me contacter
            url: "#contact"
            icon: envelope
      design:
        style: centered
        avatar_shape: circle
        animations: true
        background:
          color:
            light: "#fafafa"
            dark: "#0a0a0f"
        spacing:
          padding: ["6rem", "0", "4rem", "0"]
    
    # Portfolio filtrable - Filtrage des projets avec Alpine.js
    - block: portfolio
      id: projects
      content:
        title: "Projets phares"
        subtitle: "Une sélection de mes travaux récents"
        count: 0
        filters:
          folders:
            - projects
        buttons:
          - name: Tous
            tag: '*'
          - name: Full-Stack
            tag: Full-Stack
          - name: Front-end
            tag: Frontend
          - name: Back-end
            tag: Backend
        default_button_index: 0
        # Le lien d'archive s'affiche automatiquement s'il existe plus de projets que la valeur 'count' ci-dessus
        # archive:
        #   enable: false  # Définir sur false pour le masquer explicitement
        #   text: "Parcourir tout"  # Personnaliser le texte
        #   link: "/work/"  # URL personnalisée
      design:
        columns: 3
        background:
          color:
            light: "#ffffff"
            dark: "#0d0d12"
        spacing:
          padding: ["4rem", "0", "4rem", "0"]
    
    # Stack technique visuelle - Icônes organisées par catégorie
    - block: tech-stack
      id: skills
      content:
        title: "Stack technique"
        subtitle: "Les technologies que j'utilise"
        categories:
          - name: Téléphonie
            items:
              - name: Avaya
                icon: devicon/avaya
              - name: EnreachUp
                icon: devicon/enreach
              - name: 3CX
                icon: devicon/3cx
          - name: Réseau
            items:
              - name: Mikrotik
                icon: devicon/mikrotik
              - name: Cisco
                icon: devicon/cisco
              - name: Aruba
                icon: devicon/aruba
              - name: Fortinet
                icon: devicon/fortinet
              - name: Stormshield
                icon: devicon/stormshield
              - name: Putty
                icon: devicon/putty
          - name: OS
            items:
              - name: Windows 11
                icon: devicon/windows11
              - name: Ubuntu
                icon: devicon/ubuntu
              - name: PostgreSQL
                icon: devicon/postgresql
              - name: Redis
                icon: devicon/redis
      design:
        style: grid
        show_levels: false
        background:
          color:
            light: "#f5f5f5"
            dark: "#08080c"
        spacing:
          padding: ["4rem", "0", "4rem", "0"]
    
    # Chronologie de l'expérience
    - block: resume-experience
      id: experience
      content:
        title: Expérience
        date_format: Jan 2006
        items:
          - title: Technicien Uc et Réseaux
            company: Tech Corp
            company_url: ''
            company_logo: ''
            location: Limonest, Fr
            date_start: '2023-01-01'
            date_end: ''
            description: |2-
              * Piloté le développement d'une architecture de microservices servant plus d'1 million d'utilisateurs
              * Amélioré le temps de réponse de l'API de 40 % grâce à des optimisations
              * Encadré une équipe de 5 développeurs juniors
              * Stack technique : React, Node.js, PostgreSQL, AWS
      design:
        columns: '1'
        background:
          color:
            light: "#ffffff"
            dark: "#0d0d12"
        spacing:
          padding: ["4rem", "0", "4rem", "0"]
    
    # Articles de blog récents
    - block: collection
      id: blog
      content:
        title: Articles récents
        subtitle: 'Réflexions sur le développement web, la tech, et plus encore'
        text: ''
        filters:
          folders:
            - blog
          exclude_featured: false
        count: 3
        order: desc
      design:
        view: card
        columns: 3
        background:
          color:
            light: "#f5f5f5"
            dark: "#08080c"
        spacing:
          padding: ["4rem", "0", "4rem", "0"]
    
    # Section contact
    - block: contact-info
      id: contact
      content:
        title: Contactez-moi
        subtitle: "Travaillons ensemble"
        text: |-
          Je suis toujours intéressé par de nouveaux projets et opportunités.
          Que vous cherchiez à recruter, collaborer ou simplement dire bonjour, n'hésitez pas à me contacter !
        email: jujumions@pm.me
        autolink: true
      design:
        columns: '1'
        background:
          color:
            light: "#ffffff"
            dark: "#0d0d12"
        spacing:
          padding: ["4rem", "0", "4rem", "0"]
    
    # Carte CTA
    - block: cta-card
      content:
        title: "Ouvert aux opportunités"
        text: |-
          Je suis actuellement à la recherche de postes de **senior engineer** ou de **tech lead**.
          
          Contactons-nous pour discuter de la façon dont je peux aider votre équipe.
        button:
          text: 'Télécharger le CV'
          url: uploads/resume.pdf
          new_tab: true
      design:
        card:
          # Mode clair : dégradé pastel doux | Mode sombre : dégradé riche et profond
          css_class: 'bg-gradient-to-br from-primary-200 via-primary-100 to-secondary-200 dark:from-primary-600 dark:via-primary-700 dark:to-secondary-700'
          text_color: dark
        background:
          color:
            light: "#f5f5f5"
            dark: "#08080c"
        spacing:
          padding: ["4rem", "0", "6rem", "0"]
---
