# COMENTAIRE CSS
**Ce document détaille la structure et les styles appliqués au projet. Le code suit une approche moderne basée sur les variables CSS et la méthodologie BEM pour        garantir une maintenance facilitée.**

1. J'ai utilisé des variables CSS (:root) pour assurer une cohérence visuelle et faciliter la maintenance. La palette de couleurs suggère une thématique naturelle       ou écologique (nuances de verts et crème).1. CouleursVariableValeurUsage suggéré--color-primary#6A994ECouleur principale de la marque.--color-                        secondary#A7C957Boutons (CTA), logos et accents clairs.--color-accent#386641Éléments d'accentuation plus sombres.--color-bg#F2E8CFCouleur d'arrière-plan de la        page.--color-text#1A2E1ATexte principal (très sombre).
   
2. Espacement & BorduresEspacements (--space-) : Une échelle allant de 4px (xs) à 64px (3xl) pour gérer les marges et paddings de manière proportionnelle.Rayons de      bordure (--radius-) : Permet de définir l'arrondi des éléments, du petit bouton (4px) au bouton "pilule" (9999px).

 3.Architecture des Composants
   Pour une configuration Globale (body)
   La Largeur fixe est à 1440px (optimisé pour les écrans desktop).
   et la Mise en page j'ai utiliser de flex-direction: column avec un centrage horizontal automatique.

4. La Barre de Navigation (.navbar)
   C'est le composant principal de l'en-tête.
   La structure que j'ai Utilisé est un flexbox avec space-between pour séparer le logo de la navigation.
   La hauteur est Fixée à 80px pour une consistance visuelle.
   Le style est un  Fond sombre (--color-text-lighter) pour faire ressortir les liens clairs.

6. Typographie
   La police que j'ai Utilisé Libre Baskerville (Serif), apportant un aspect classique et élégant.
   Le logo est une image en forme  d'un bloc carré de 58px avec des coins arrondis (radius-md).
   Le titres etait complexes donc j'ai utiliser des variantes (--erte, --plan--b) pour permettre un titrage avec different couleur au sein d'un même bloc.

7. Bouton CTA (.btn__cta)
   Le bouton d'appel à l'action est conçu pour une visibilité maximale :
   avec un arrière-plan : Vert clair (--color-secondary).
   un comporte un padding interne de 10px 16px pour une zone de clic confortable.
   la typographie interne est un texte lien centré avec une taille de police de 14px.
   
8.Méthodologie de Nommage
  Le projet respecte la convention BEM (Block Element Modifier) pour éviter les conflits de styles :
  Block : .navbar (Le composant parent)
  Element : .navbar__link (Un enfant du bloc)
  Modifier : .navbar__title--action--erte, navbar__title--plan--b et navbar__link--nam--btn (Une version spécifique pour l'élément)
