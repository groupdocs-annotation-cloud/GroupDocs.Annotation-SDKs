---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Annotation"
product_tag: "annotation"
platform: "PHP"
platform_tag: "php"

############################# Head ############################
head_title: "Python Document & Image Annotation Cloud SDK for PDF Word Excel HTML"
head_description: "Python Cloud SDK for managing images and document annotations. Use REST APIs to easily manipulate PDF, image, HTML, Word, Excel, & email annotation."

############################# Header ############################
title: "Let's Annotate in Python with RESTful API"
description: "REST API & Cloud SDK for Python to build online document & image annotation tools with support for text & image annotation options. Let's annotate!"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Annotation Cloud SDK for Python"
        image: "/sdk/272x272/groupdocs_annotation-for-python.webp"
        product: "GroupDocs.Annotation"
        platform: "Python"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Overview"

            # button loop
            - link: "#features"
              text: "Features"


            # button loop
            - link: "https://docs.groupdocs.cloud/annotation/release-notes/"
              text: "Release Notes"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://github.com/groupdocs-annotation-cloud/groupdocs-annotation-cloud-python"
        link_learn: "https://docs.groupdocs.cloud/annotation/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Annotation Cloud SDK for Python RESTful APIs is all you need to build document annotator tools in Python. Your application will be able to add annotations, watermark overlays, text replacements, redactions, sticky notes and text markups to the business documents of all popular formats such as, PDF, Microsoft Word, Excel, PowerPoint, Outlook, images other formats. Rapidly develop Annotation applications in Python using our SDK that works as a wrapper around Python APIs and makes the solution cross-platform compatible. Support for 3rd party cloud storage providers, e.g., Amazon S3, Windows Azure, Dropbox and others is also provided.

    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          PyPi package is required for communicating with the GroupDocs.Annotation Cloud SDK API for Python.
      
        left:
          enable: true
          icon: "fas fa-crop"
          title: "Figure Annotations"
          content: |
            * Area annotation
            * Point annotation
            * Area redaction
            * Polyline
            * Pointer/arrow
            * Watermark
            * Distance
        right:
          enable: true
          icon: "fas fa-file-alt"
          title: "Text Annotations"
          content: |
            * Annotation
            * Replacement
            * Redaction
            * Strikethrough / Underline
            * Typewriter
            
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Annotation Cloud SDK APIs support following file formats:



        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office Formats"
              content: |
                * **Word**: DOC, DOCX, DOCM, DOT, DOTX, RTF
                * **Excel**:  XLS, XLSX, XLSM, XLSB, CSV
                * **PowerPoint**: PPT, PPTX, PPS, PPSX
                * **Visio**: VSD, VSDX, VSS, VST

        right:
          enable: true
          table:
            # table loop
            - title: "Other Formats"
              content: |
                * **OpenDocument**: ODT, OTT, ODS, ODP
                * **Image Files**: BMP, PNG, JPG, JPEG, TIFF, TIF, GIF
                * **Fixed Layout**: PDF
                * **Web**: HTM, HTML
                * **Email**: EML
                * **CAD**: DWG, DXF


      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Annotation set of SDK REST APIs is not dependent on your local operating system or database. We offer our SDK APIs in numerous programming languages and with frequent new additions.
      
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Operating Systems"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Supported Frameworks"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Development Environments"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Build Automation Tool"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "Advanced Document Annotation REST API Features"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Support for Multiple File Formats"

      # feature loop
      - icon: "fas fa-desktop"
        content: "Import Annotation Information from Document & Return the List of Imported Annotations"

      # feature loop
      - icon: "fas fa-comment"
        content: "Export/Add Annotation to a Document & Retrieve the Resultant Document as Stream"
      
      # feature loop
      - icon: "fas fa-puzzle-piece"
        content: "Render Document Pages to Images and Retrieve Images’ Links"

      # feature loop
      - icon: "fas fa-retweet"
        content: "Retrieve Link to Previously Generated Image by Page Number of Annotated Document"

      # feature loop
      - icon: "fas fa-archive"
        content: "Render Document to PDF, Save Resultant Document to Storage & Fetch its Link"

      # feature loop
      - icon: "fas fa-file-pdf"
        content: "Render Document to PDF as an Output Stream"

      # feature loop
      - icon: "fas fa-eye-slash"
        content: "Add Text Redaction Annotation in Slides"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Add Annotations to Header/Footer of Microsoft Word Documents"
    
    more_feature:
      # more_feature_loop
      - title: "Easy Integration"
        content: "Integrating GroupDocs.Annotation Cloud SDK into your Python applications is very easy. No installation is required on the server or client side. Just create an account at GroupDocs.Cloud to get App SID & key. Following example shows how easy it is to import annotation information using Python:"

      # more_feature_loop
      - title: "Add Area Annotation To Document - Python"
        content: |
          
          ```python
            # Get your App SID and App Key at https://dashboard.groupdocs.cloud (free registration is required).
            # For complete examples and data files, please go to https://github.com/groupdocs-annotation-cloud/groupdocs-annotation-cloud-python
            app_sid = "XXXX-XXXX-XXXX"
            app_key = "XXXXXXXXXXXX"

            # Create instance of the API.
            api = groupdocs_annotation_cloud.AnnotationApi.from_keys(app_sid, app_key)
            path = "FolderName" + "MyDocument.pdf"

            a = AnnotationInfo()
            a.annotation_position = Point()
            a.annotation_position.x = 852
            a.annotation_position.y = 59
            a.box = Rectangle()
            a.box.x = 375
            a.box.y = 59
            a.box.width = 88
            a.box.height = 37
            a.type = "Area"
            a.creator_name = "Anonym A."

            request = groupdocs_annotation_cloud.PostAnnotationsRequest(path, a)
            response = api.post_annotations(request)
            print(response)
          ```
      # more_feature_loop
      - title: "Support for Numerous Annotation Types"
        content: "Using GroupDocs.Annotation Cloud SDK for Python, you can work with diverse types of annotations. The two basic types are; Text Annotations and Figure Annotations.

        While using text-based annotation, you can add text comments to selected text; highlight which text should be replaced with what, hide confidential text using text redaction, highlight text with strikethroughs/underlines, and add sticky notes with rich text.

        While working with figure annotations, you can add notes to an area highlighted with a rectangle (Area Annotation), add notes to any point in the document (Point Annotation), hide confidential parts of an image or text (Area Redaction), draw freehand lines and shapes (Polyline), arrows pointing to an object (Pointer/Arrow), create text-based watermark overlays (Watermark), and measure the distance between any objects in a document (Distance Annotation)."

      # more_feature_loop
      - title: "Easy Customization"
        content: "GroupDocs.Annotation Cloud SDK for Python is 100% tested and out of the box running. The SDK is open source and has an MIT license. You can use it, and even customize it for absolutely free of charge."
      # more_feature_loop
      - title: "Interactive API Explorer"
        content: "Using our Swagger based API explorer; you can try out GroupDocs.Annotation Cloud SDK for Python right away in your browser. This interactive API explorer gives you information about all the resources that the API offers. You can also try your desired operation by interactively providing required parameters."
      

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Annotation Cloud Product Family also includes SDKs for other popular languages as listed below:"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for cURL"
          image: "/sdk/272x272/groupdocs_annotation-for-curl.webp"
          product: "GroupDocs.Annotation"
          platform: "cURL"
          link: "/annotation/curl/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for .NET"
          image: "/sdk/272x272/groupdocs_annotation-for-net.webp"
          product: "GroupDocs.Annotation"
          platform: ".NET"
          link: "/annotation/net/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for Java"
          image: "/sdk/272x272/groupdocs_annotation-for-java.webp"
          product: "GroupDocs.Annotation"
          platform: "Java"
          link: "/annotation/java/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for PHP"
          image: "/sdk/272x272/groupdocs_annotation-for-php.webp"
          product: "GroupDocs.Annotation"
          platform: "PHP"
          link: "/annotation/php/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for Python"
          image: "/sdk/272x272/groupdocs_annotation-for-python.webp"
          product: "GroupDocs.Annotation"
          platform: "Python"
          link: "/annotation/python/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for Ruby"
          image: "/sdk/272x272/groupdocs_annotation-for-ruby.webp"
          product: "GroupDocs.Annotation"
          platform: "Ruby"
          link: "/annotation/ruby/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for Node.js"
          image: "/sdk/272x272/groupdocs_annotation-for-node.webp"
          product: "GroupDocs.Annotation"
          platform: "Node.js"
          link: "/annotation/nodejs/"

############################# Back to top ###############################
back_to_top:
  enable: true
---