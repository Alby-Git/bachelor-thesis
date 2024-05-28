<a name="readme-top"></a>

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://galaxyproject.org/">
    <img src="images/galaxy_project_logo.png" alt="Logo" width="250" height="80">
  </a>

<h2 align="center">Bachelor's Project </h2>
  <p align="center">
    Port, improve, and benchmark read-based MGnify analysis pipeline for microbiome data using the Galaxy framework
  <h4 align="center"> by Albert Ratschinki </h4>
    <br />
    <a href="https://github.com/Alby-Git/bachelor-thesis"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/Alby-Git/bachelor-thesis/tree/main/tools/taxpasta"><strong>Taxpasta</strong></a> 
    ·
    <a href="https://github.com/Alby-Git/bachelor-thesis/tree/main/tools/opal"><strong>Opal</strong></a> 
    <br />
    <br />
    <a href="https://github.com/Alby-Git/bachelor-thesis/issues">Report Bug</a>
    ·
    <a href="https://github.com/Alby-Git/bachelor-thesis/issues">Request Feature</a>
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#preparations">Preparations</a></li>
        <li><a href="#using-taxpasta-and-opal-in-galaxy">Using Taxpasta and Opal in Galaxy</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#planemo-101">Planemo 101</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project

From October 16th to January 16th, I embarked on a bachelor's project as part of my Bachelor's degree at the Professorship for Bioinformatics. Supervised by [Paul Zierep](https://github.com/paulzierep), my task was to port, improve, and benchmark the read-based MGnify analysis pipeline for microbiome data using the Galaxy framework.

### Project Overview

Microbiome data analysis is a complex field, necessitating advanced computational tools and methodologies. My project centered on the [MGnify V5 Raw reads Pipeline](https://www.ebi.ac.uk/metagenomics/pipelines/5#raw), a well-regarded pipeline in microbiome data analysis.

A significant part of my project involved wrapping the tools [Taxpasta](https://github.com/pelkmanslab/taxpasta) and [Opal](https://github.com/OpenAPI-Specification/Opal) for integration into the [Galaxy platform](https://galaxyproject.org/). This integration was crucial as it allows the full workflow of the MGnify V5 pipeline to be executed within Galaxy, making it accessible for a broader range of researchers and facilitating ease of use.

<br>
<div align="center" style="width: 80%; margin: auto;">
  <figure>
    <a href="https://www.ebi.ac.uk/metagenomics/pipelines/5#raw">
      <img src="images/mgnifyV5.png" alt="MGnify Version 5 Logo" style="width: 100%; height: auto; border: 5px solid #7b2cbf;">
    </a>
    <figcaption>An illustration of the MGnify V5 pipeline</figcaption>
  </figure>
</div>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started

Follow these steps to use Taxpasta and Opal on the Galaxy platform and prepare for the upcoming integration.

### Preparations

Before starting, ensure you have created an account on [Galaxy](https://usegalaxy.eu/). Galaxy offers a web-based platform with a wide array of bioinformatics tools for research.

### Using Taxpasta and Opal in Galaxy

Taxpasta and Opal are going to be integrated into Galaxy and can be used for preprocessing and analyzing microbiome sequencing data. Here's how to use them:

1. **Create a Galaxy Account:**
   - Visit [usegalaxy.eu](https://usegalaxy.eu/) and create an account if you don’t already have one.

2. **Find the Tools:**
   - Once logged in to Galaxy, search for "Taxpasta" and "Opal" in the tool search bar.

3. **Upload Data:**
   - Upload your microbiome sequencing data to Galaxy.

4. **Configure the Tools:**
   - Select Taxpasta or Opal from the list of tools and configure them according to your specific requirements for your data.

5. **Run the Tools:**
   - Execute the tools and wait for the results. Taxpasta and Opal will process your data appropriately, preparing it for further analysis.

### Future Integration of mOTUs

Currently, mOTUs is not yet directly integrated into Galaxy, but work is underway to make this tool available soon. Once mOTUs is integrated into Galaxy, it will enable efficient and user-friendly metagenomic analyses. Keep an eye on updates in our repository to stay informed about the integration of mOTUs.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- USAGE -->
## Usage

The tools and methodologies developed in this project can be applied in various ways to facilitate and enhance microbiome data analysis. Below are some examples of how these tools can be utilized within the Galaxy framework:

### Example Use Cases:

1. **Microbiome Data Preprocessing with Taxpasta:**
   - Utilize Taxpasta for the preprocessing of microbiome sequencing data. This includes steps like taxonomic classification and data aggregation.
   - Example Workflow:    
      - After uploading your sequencing data to Galaxy, select Taxpasta from the tool menu.
      - Configure the tool parameters according to your experiment's requirements.
      - Execute the tool to process the data. The output will be a taxonomic profile, ready for further analysis.

2. **Metagenomic Analysis with Opal:**
   - Deploy Opal for advanced metagenomic analysis. This tool helps in performing comprehensive data analyses and visualizations.
   - Example Workflow: 
      - Start with preprocessed reads.
      - Select Opal from the Galaxy tool menu.
      - Input your data into Opal and specify the analysis parameters.
      - Run the tool. Opal will output detailed analyses and visualizations of the microbial community in your sample.

### Integrating Tools in Galaxy:

- **Galaxy Environment:** 
  - [Galaxy](https://galaxyproject.org/) is an open, web-based platform for computational biomedical research. It allows users to reproduce and share analyses.
  - Within Galaxy, tools like Taxpasta and Opal can be integrated to streamline and simplify the microbiome data analysis pipeline.

### Additional Resources and Documentation:

- For detailed instructions, use cases, and tutorials on how to use these tools in Galaxy, please refer to the [Galaxy Training Network](https://training.galaxyproject.org/training-material/).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ROADMAP -->
## Roadmap

**Taxpasta**
- [ ] **Understanding Taxpasta**
  - Research [Taxpasta](https://github.com/pelkmanslab/taxpasta) tool and its mechanisms.
- [ ] **Blueprint for Taxpasta**
  - Develop a plan for wrapping Taxpasta using Planemo.
- [ ] **Implement Taxpasta in Galaxy**
  - Successfully wrap Taxpasta and demonstrate its functionality on Galaxy.
- [ ] **Contribute to IUC**
  - Prepare and submit a pull-request to integrate Taxpasta into the IUC main branch. (Here)[https://github.com/galaxyproject/tools-iuc/pull/5719]

**Opal**
- [ ] **Explore Opal**
  - Learn about the Opal tool and its applications.
- [ ] **Plan Opal Integration**
  - Design a strategy for incorporating Opal into Galaxy.
- [ ] **Galaxy Implementation**
  - Execute the integration of Opal into the Galaxy platform.
- [ ] **Testing and Validation**
  - Ensure Opal works seamlessly within Galaxy; perform tests.
- [ ] **Contribute to bgruening-galaxytools**
  - Prepare and submit a pull-request to integrate Opal into the galaxytools branch from bgruening main branch.
  
- [ ] **Understand Data Manager Requirements**
  - Study the specific needs for a data manager for Opal.
- [ ] **Development Plan**
  - Draft a comprehensive plan for developing the Opal data manager.
- [ ] **Implementation**
  - Develop and integrate the data manager into the Galaxy ecosystem.
- [ ] **Optimization and Review**
  - Optimize for performance and user-friendliness; prepare for peer review.

For a full list of proposed features and known issues, see the [open issues](https://github.com/Alby-Git/bachelor-thesis/issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- PLANEMO 101 -->
## Planemo 101

### Installation

1. **Install Planemo:**

   - For more information, visit the [Planemo documentation](https://planemo.readthedocs.io/en/latest/).

### Test

1. **Running Tests:**

   - To test your Galaxy tools, use the following Planemo command:
     ```sh
     planemo test --galaxy_root /path/to/galaxy_root my_tool.xml
     ```

### Serve

1. **Running a Local Galaxy Server:**

   - To serve your tools in a local Galaxy instance, use this command:
     ```sh
     planemo serve --galaxy_root /path/to/galaxy_root my_tool.xml
     ```

   - This will start a local Galaxy server where you can test your tools in a real Galaxy environment.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

Special thanks to:

* **Paul Zierep:** For his mentorship and expertise in guiding the development and implementation of the project, particularly in the areas of bioinformatics and data analysis.
* **Rand:** For the significant assistance with Planemo and Taxpasta, facilitating key aspects of the project's development.
* **Galaxy Project Team:** For providing an excellent platform for bioinformatics research.
* **Taxpasta and Opal Developers:** For their contributions to microbiome data analysis tools.

<p align="right">(<a href="#readme-top">back to top</a>)</p>
