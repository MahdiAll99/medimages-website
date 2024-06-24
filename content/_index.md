---
title: 'Home'
date: 2023-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: hero
    content:
      title: Open the World of Radiomics
      text:  An all-in-one open-source software designed to enhance synergy between computer scientists and clinical researchers in the field of radiomics.
      primary_action:
        text: Get Started
        url: https://medomics-udes.gitbook.io/medimage-app-docs
        icon: rocket-launch
      secondary_action:
        text: Explore tutorials
        url: https://youtube.com/playlist?list=PLEPy2VhC4-D5Eg-UxRyTtmUZRh-D5m_Ru&si=QnNFQe5-oRVHmoh8
      announcement:
        text: Announcing the first release
        link:
          text: soon...
          url: https://github.com/MEDomics-UdeS/medimage-app/releases
    design:
      spacing:
        padding: [0, 0, 0, 0]
        margin: [0, 0, 0, 0]
      # For full-screen, add `min-h-screen` below
      css_class: "dark"
      background:
        image:
          # Add your image background to `assets/media/`.
          filename: medical-ai.jpg
          filters:
            brightness: 0.5

  - block: markdown
    id: design
    
  - block: hero
    design:
      spacing:
        padding: [100, 0, 0, 0]
        margin: [0, 0, 0, 0]
      # For full-screen, add `min-h-screen` below
      css_class: "dark"
      background:
        video:
          # Add your image background to `assets/media/`.
          filename: Promotional_Video.mp4

  - block: features
    id: features
    content:
      title: Features
      text: "Transforming medical images into insightful knowledge: explore, analyze, and extract with MEDimage."
      items:
        - name: Easy & Fast
          icon: sparkles
          description: An all-in-one solution for medical image analysis that enables easy radiomics feature extraction and offers tailored functionalities for model training to streamline your experiments.
        - name: No-Code
          icon: code-bracket
          description: You're not a fan of coding? the solution offers an intuitive interface, eliminating the need for coding.
        - name: Compliant
          icon: check-badge
          description: Our package adheres to the radiomics extraction international standards set by the [**IBSI**](https://theibsi.github.io/).
  
  - block: markdown
    id: architecture
    content:
      title: Software architecture
      text: |
        <div style="text-align: center">
        <p> MEDimage solution for medical image analysis is based on two integral components, a <u><b><a href="https://github.com/MEDomics-UdeS/medimage-app/">code-free interface</a></b></u> and a <u><b><a href="https://github.com/MEDomics-UdeS/MEDimage">code-base package</a></u></b> to push for more synergy between inter-disciplinary teams. Using the code generation feature, users can transition between the two components. The global architecture of MEDimage is illustrated below. </p>
        <br></br>
          <img src="https://github.com/MahdiAll99/medimages-website/blob/main/assets/media/global_architecture.png?raw=true" style="max-width:none;
            width:1700px; height: auto;" alt="MEDimage Workflow" style="width: 1000px; height: auto;">
        </div>
  
  - block: markdown
    id: design
    content:
      title: MEDimage package workflow
      text: |
        <div style="text-align: center">
        <p> The following figure depicts the MEDimage <u><b><a href="https://github.com/MEDomics-UdeS/MEDimage">python package</a></u></b> architecture, a modular solution that ensures an easy manipulation and modification of the code.</p>
        <br></br>
          <img src="https://github.com/MahdiAll99/medimages-website/blob/main/assets/media/MEDimages-Workflow.png?raw=true" style="max-width:none;
            width:1500px; height: auto;" alt="MEDimage Workflow" style="width: 1000px; height: auto;">
        </div>
  
  - block: cta-image-paragraph
    id: solutions
    content:
      items:
        # Build model
        - title: Analyze your images now
          text: As easy as 1, 2, 3!
          feature_icon: check
          features:
            - "Drag-Drop style interface for easy feature extraction and model training"
            - "All-In interface for medical image analysis"
            - "No Python knowledge required"
          # Upload image to `assets/media/` and reference the filename here
          image: MEDimages-interface.png
          button:
            text: Get Started
            url: https://medomics-udes.gitbook.io/medimage-app-docs/quick-start
        # Tutorials
        - title: Resources
          text: We offer a range of resources to help you get started.
          feature_icon: bolt
          features:
            - "[**Comprehensive code documentation website**](https://medimage.readthedocs.io/)."
            - "[**Comprehensive interface documentation website**](https://medomics-udes.gitbook.io/medimage-app-docs)."
            - "[**Tutorials and code examples**](https://github.com/MEDomics-UdeS/MEDimage/tree/main/notebooks)"
            - "[**Guided video tutorials for step-by-step learning**](https://www.youtube.com/playlist?list=PLEPy2VhC4-D5Eg-UxRyTtmUZRh-D5m_Ru)"
          # Upload image to `assets/media/` and reference the filename here
          image: MEDimages-resources.png
          
          # Problems
        - title: Errors & Bugs
          text: For any errors or bugs, please report them to us. We will be happy to help.
          # Upload image to `assets/media/` and reference the filename here
          image: MEDimages-error.png
          button:
            text: Report an issue
            url: https://github.com/MEDomics-UdeS/medimage-app/issues
    design:
      css_class: "bg-gray-100 dark:bg-gray-900"
  - block: markdown
    id: FAQ
    content:
      title: FAQ
      text: "
      <ul>
        <li><strong>Q: Which medical image formats are compatible with MEDimage?</strong></li>
          <ul>
            <li>A: MEDimage is compatible with widely used formats such as DICOM and NIfTI, commonly employed for the storage and transmission of medical images.</li>
          </ul>
        </li>
        <li><strong>Q: Does MEDimage support customized features extraction</strong></li>
          <ul>
            <li>A: Customized features extraction is supported for individual scans. However, for batch extraction, features are processed following the IBSI workflow.</li>
          </ul>
        </li>
      </ul> 
      "

---
