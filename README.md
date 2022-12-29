
# Site settings
title: 课题组
description: "关于课题组的故事"
url: "https://projectpages.github.io"




# Secondary Parameters
baseurl: "/课题组"
header-img: img/home1.jpg
headercolor: "#FFFFFF"
logo: /project-pages/img/logos/Project-Pages-New-Logo-Inverted.png

# Tertiary Parameters
github_username:  课题组
project_repository: 课题组
disqus_shortname: 课题组
g-analytics: UA-75881392-1
altmetric: true

# Build settings
gems: [jekyll-paginate]
markdown: kramdown
highlighter: rouge
permalink: pretty
paginate: 10
exclude: ["less","node_modules","Gruntfile.js","package.json","README.md"]

# Jekyll Settings

defaults:
  -
    scope:
      path: "projects"
      type: "pages"
    values:
      layout: "project"
      header-img: "img/home1.jpg"

# Prose Settings
prose:
  ignore: ['feed.xml', '/stl', '/ply', '/js', '/plugin', '/lib', '/projectors', '_layouts', '/_includes', 'Gruntfile.js', 'package.json', 'proselinks.jsonp', 'ppanchor.matin', '.gitignore', '/search', '/css', '/img', 'favicon.png','_data/*.json','LICENSES.md','README.md','colorscheme.scss','members.html','mentions.html','index.html']
  siteurl: 'http://projectpages.github.io/project-pages/'
  ispp: true
  media: 'img'
  metadata:
    projects:
      - name: "title"
        field:
          element: "text"
          label: "Title"
          value: ""
      - name: "description"
        field:
          element: "text"
          label: "Description"
          value: ""
      - name: "category"
        field:
          element: "text"
          label: "Project"
          value: ""           
    _posts:
      - name: "subtitle"
        field:
          element: "text"
          label: "Sub-Title (Short Description)"
          value: ""
      - name: "layout"
        field:
          element: "select"
          label: "Choose Layout"
          placeholder: "Layouts"
          options:
            - name: "Post"
              value: "post"
            - name: "Slide"
              value: "slide"
            - name: "Projector"
              value: "projector"
            - name: "Notebook"
              value: "notebook"
            - name: "Ply Surface"
              value: "plysurface"
      - name: "title"
        field:
          element: "text"
          label: "Title"
          value: ""
      - name: "author"
        field:
          element: "text"
          label: "Author"
          value: ""
      - name: "tags"
        field:
          element: "text"
          label: "Tags (seperate with whitespace)"
          value: ""
      - name: "category"
        field:
          element: "text"
          label: "Project"
          value: ""    
      - name: "horizontal"
        field:
          element: "hidden"
          value: </section></section><section markdown="1" data-background="http://projectpages.github.io/project-pages/img/slidebackground.png"><section markdown="1">
      - name: "vertical"
        field:
          element: "hidden"
          value: </section><section markdown="1">
      - name: "slideinit"
        field:
          element: "hidden"
          value: <section markdown="1" data-background="http://projectpages.github.io/project-pages/img/slidebackground.png"><section markdown="1">
      - name: "theme"
        field:
          element: "select"
          label: "Theme (Slide)"
          placeholder: "Theme (Slide)"
          options:
            - name: "Beige"
              value: "beige"
            - name: "Blood"
              value: "blood"
            - name: "Moon"
              value: "moon"          
            - name: "Night"
              value: "night"
            - name: "Sky"
              value: "sky"
            - name: "Solarized"
              value: "solarized"             
      - name: "trans"
        field:
          element: "select"
          label: "Transition (Slide)"
          placeholder: "Transition (Slide)"
          options:
            - name: "Cube"
              value: "cube"
            - name: "Page"
              value: "page"
            - name: "Concave"
              value: "concave"          
            - name: "Linear"
              value: "linear"
            - name: "Fade"
              value: "fade"
            - name: "None"
              value: "none"             
      - name: "visualworkflow"
        field:
          element: "checkbox"
          label: "Visual Workflow Chart (Some Layouts)"
          value: "true"
