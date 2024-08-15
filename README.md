\documentclass{article}
\usepackage{geometry}
\geometry{margin=1in}
\setlength{\parskip}{0.5em}
\setlength{\parindent}{0pt}

\title{LAB 2 - Wildfire Spread Dynamics}
\author{Tanav Thanjavuru, Simran Gill, Ozkan Meric Ozcan}
\date{July 23, 2024}

\begin{document}

\maketitle

\section*{Project Summary}
This project investigates the dynamics of wildfire spread in the northeast region of Portugal. The focus is on understanding the relationship between the Fine Fuel Moisture Code (FFMC) and the Initial Spread Index (ISI), which are crucial indicators of fire behavior. The analysis aims to determine how FFMC influences the speed at which wildfires spread.

\section*{Methodology}
\begin{itemize}
    \item **Data Source:** The "Forest Fires" dataset from the UCI Machine Learning Repository, consisting of 517 instances with 13 features related to climate and physical factors in the Montesinho natural park.
    \item **Data Preparation:** The dataset was split into an exploration set (30\%) and a confirmation set (70\%). Outliers were detected and removed to ensure data quality.
    \item **Modeling Approach:**
    \begin{itemize}
        \item A simple linear regression model was initially used to explore the relationship between FFMC and ISI.
        \item A log-linear regression model was then applied to address skewness in the data and improve model fit.
    \end{itemize}
\end{itemize}

\section*{Key Results}
\begin{itemize}
    \item The log-linear regression model showed a strong relationship between FFMC and ISI, with an adjusted R\textsuperscript{2} of 0.74.
    \item The log transformation improved model stability and linearity, providing a better fit compared to the simple linear model.
    \item The FFMC was found to be a significant predictor of wildfire spread, as measured by ISI.
\end{itemize}

\section*{Conclusion}
The findings suggest that FFMC is a robust indicator for predicting the speed of wildfire spread in the studied region. The results highlight the importance of monitoring FFMC to assess wildfire risks, which could aid in better fire management and prevention strategies.

\section*{References}
\begin{itemize}
    \item Howard, B. C. (2023, October 4). \textit{How to live with mega-fires: Portugal’s forests may hold the secret}. National Geographic. Retrieved from \url{https://www.nationalgeographic.com/science/article/how-to-live-with-mega-fires-portugal-forests-may-hold-secret}
    \item Sampson, L. (2024, July 18). \textit{Where are the Portugal wildfires and is it safe to travel?} The Times. Retrieved from \url{https://www.thetimes.com/travel/advice/where-are-the-portugal-wildfires-is-it-safe-to-travel-ttflwnmnr}
\end{itemize}

\end{document}
