Are All Tipping Points Predictable?

A Test of Early Warning Signal Theory on Holocene Climate Events

Author: Gururaj H C
License: MIT License
Project Overview

This repository contains the code and data for the research paper: "Are All Tipping Points Predictable? A Test of Early Warning Signal Theory on Three Distinct Holocene Climate Events."

This project evaluates Early Warning Signal (EWS) theory using high-resolution palaeoclimate data. By analyzing oxygen isotope records around major Holocene climate transitions, we assess the robustness of statistical indicators (autocorrelation and variance) across different detrending methods and window sizes.
Dataset

    Source: NGRIP ice core

            
    δ18Oδ18O

          

    record.

    File: dataset.txt (Tab-separated values: age_calBP, d18O_vsmow).

    Events Analyzed:

        Younger Dryas Termination (~11,700 BP)

        8.2k Event (~8,200 BP)

        Holocene Thermal Maximum Onset (~6,500 BP)

Methodology

The Python notebook implements the following pipeline:

    Preprocessing: Extraction of time windows (

            
    ±2000±2000

          

    years) around specific transitions.

    Detrending: Application of four distinct methods:

        Gaussian Kernel Smoothing

        Savitzky-Golay Filter

        Univariate Spline Fitting

        First Differencing

    Metric Calculation: Rolling Lag-1 Autocorrelation (AR1) and Variance.

    Significance Testing: Kendall’s

            
    ττ

          

    trend strength evaluated against 300 phase-randomized surrogate series.

Key Findings

    Holocene Thermal Maximum: Displays a robust, consistent autocorrelation signal across methods.

    Younger Dryas: Shows strong signals but is sensitive to window size selection.

    8.2k Event: Lacks a consistent early warning signal, highlighting the limitations of EWS for rapid, externally forced transitions.

Usage

    Ensure dataset.txt is in the same directory as the notebook.

    Run Are_All_Tipping_Points_Predictable.ipynb.

    Outputs will be generated in the Figures/ folder.

Preprint

The preprint for this work is available at: https://eartharxiv.org/repository/view/9558/
