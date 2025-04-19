# A/B Testing Analysis: Landing Page Conversion

## Table of Contents
1. [Project Overview](#project-overview)  
2. [Data](#data)  
3. [Repository Structure](#repository-structure)  
4. [Getting Started](#getting-started)  
   - [Option A: Start from Blank](#option-a-start-from-blank)  
   - [Option B: Clone Existing Repo](#option-b-clone-existing-repo)  
5. [Installation & Setup](#installation--setup)  
6. [How to Run](#how-to-run)  
7. [Key Findings](#key-findings)  
8. [Next Steps](#next-steps)  
9. [Author](#author)  

---

## Project Overview
This project evaluates whether a redesigned landing page (treatment group) leads to a higher conversion rate compared to the original page (control group). We load session and purchase data, perform exploratory analysis, visualize conversion rates, and run a two‑sample z‑test to assess significance.

## Data
- **archive/control_group.csv** – Users exposed to the original landing page  
- **archive/test_group.csv** – Users exposed to the new landing page  

Each CSV includes:  
- `User ID`  
- `# of Session`  
- `# of Purchase`

## Repository Structure
