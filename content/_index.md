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
      text:  An open-source python package revolutionizing the processing of medical images and extracting radiomics features for enhanced insights.
      primary_action:
        text: Get Started
        url: https://github.com/MahdiAll99/MEDimage
        icon: rocket-launch
      secondary_action:
        text: Read the docs
        url: https://medimage.readthedocs.io/en/latest/
      announcement:
        text: Announcing the release of version 1.
        link:
          text: Read more
          url: https://github.com/MahdiAll99/MEDimage/releases
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
    content:
      title: MEDimages Workflow
      text: "![](https://github.com/MahdiAll99/medimages-website/blob/main/assets/media/MEDimages-Workflow.png?raw=true)"
  - block: features
    id: features
    content:
      title: Features
      text: "Transforming Medical Images into Insightful Knowledge: Explore, Analyze, and Extract with MEDimages."
      items:
        - name: Automated
          icon: wrench
          description: Automated data processing, extraction of regions of interest (ROI), organization of metadata, and feature extraction.
        - name: Easy & Fast
          icon: sparkles
          description: Effortlessly achieve rapid and efficient medical image processing, radiomics feature extraction, and coding with MEDimages, leveraging parallelization techniques to streamline the development of medical image analysis.
        - name: No-Code
          icon: code-bracket
          description: You're not a fan of coding? navigate the robust features of MEDimages using our intuitive interface app, eliminating the need for coding while ensuring powerful medical image analysis and radiomics extraction.
        - name: Versatile
          icon: rectangle-group
          description: We provide a range of functionalities tailored to your requirements, encompassing image processing, feature extraction, model training, and analysis.
        - name: Resources
          icon: circle-stack
          description: The package provides diverse resources, including tutorials, code examples, and more, to aid users in getting acquainted with its functionalities.
        - name: Compliant
          icon: check-badge
          description: Our package adheres to the radiomics extraction international standards set by the [**IBSI**](https://theibsi.github.io/).
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
            url: https://github.com/MahdiAll99/MEDimage
        # Tutorials
        - title: Resources
          text: We offer a range of resources to help you get started.
          feature_icon: bolt
          features:
            - "Comprehensive documentation website"
            - "In-depth tutorials and code examples"
            - "Guided video tutorials for step-by-step learning"
          # Upload image to `assets/media/` and reference the filename here
          image: MEDimages-resources.png
          button:
            text: Check our tutorials
            url: https://medimage.readthedocs.io/en/latest/tutorials.html
          # Problems
        - title: Errors & Bugs
          text: For any errors or bugs, please report them to us. We will be happy to help.
          # Upload image to `assets/media/` and reference the filename here
          image: MEDimages-error.png
          button:
            text: Report an issue
            url: https://github.com/MahdiAll99/MEDimage/issues
    design:
      css_class: "bg-gray-100 dark:bg-gray-900"
  - block: markdown
    id: FAQ
    content:
      title: FAQ
      text: "
      <ul>
        <li><strong>Q: Which medical image formats are compatible with MEDimages?</strong></li>
          <ul>
            <li>A: MEDimages is compatible with widely used formats such as DICOM and NIfTI, commonly employed for the storage and transmission of medical images.</li>
          </ul>
        </li>
        <li><strong>Q: Does MEDimages support customized features extraction</strong></li>
          <ul>
            <li>A: Customized features extraction is supported for individual scans. However, for batch extraction, features are processed following the IBSI workflow.</li>
          </ul>
        </li>
      </ul> 
      "

---
