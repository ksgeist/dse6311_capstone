# Welcome to Capstone

The Capstone is an opportunity to bring together skills from your MSDS coursework by applying them to an end-to-end data science project. **You are not expected to arrive knowing how to do every part of the project already**. Learning new methods, strengthening your technical judgment, and applying feedback are expected parts of Capstone.

You will have opportunities to learn throughout the course through asynchronous instructional materials, examples, project work, feedback, peer review, and discussion. The goal is to make that learning timely and useful: you will encounter concepts as you need them, apply them to your project, and document what you learn.

By the end of eight weeks, your goal is to produce a **defensible, reproducible analysis and a professional GitHub portfolio** that communicates what you did, why you did it, what you found, and what the limitations are.

## How to use this roadmap

Each week has a focus and a milestone. The milestones build on one another, so the work you do early should contribute to your final project rather than become a series of disconnected assignments.

1. ***Review the weekly instructions and asynchronous learning materials at the start of each week.*** These will be posted by Tuesday mornings, if not sooner, in most cases. I will try to have materials available to you the weekend before since I know many of you work on this on weekends (as do I!).

2. ***Work with your project and data throughout the week as much as you can.*** Do not wait until a deliverable is due to begin the work.

3. ***Use your weekly standup discussion post to your advantage.*** This is not just busy work! Use this time to communicate progress, next steps, and blockers both to me and to your team. You may use a video if you wish, but video is not required. These are due by 11:59PM EST on Tuesday **in lieu of synchronous class attendance**.

4. ***Ask for help when you need it.*** A useful part of Capstone is learning to identify what you do not yet know, find appropriate resources, test your understanding, and use feedback. Notably, I will be checking in with you 1:1 each week through your assignment - your Individual Reflections - but if things are going well, you need only say that and keep going.

5. ***Keep your GitHub portfolio up to date.*** As the project develops, do not wait to update your `README`, organize your repo, or create any necessary documentation. You will find it much easier to do this as you go rather than wait until the end.

# A Note on Learning and Expectations

You are expected to keep learning throughout Capstone. The course is not simply a test of whether you already know every technique you may need. You will encounter problems that require you to revisit concepts, consult instructional materials, test alternatives, ask questions, and respond to feedback.

At the same time, you are responsible for engaging with the materials, applying what you learn, documenting your decisions, and seeking help early enough to act on it. My role is project manager, mentor, and instructor: I am here to guide your progress, provide feedback, and help you make sound decisions, but I will not be prescribing every technical choice in advance. 
Furtherm the goal is not simply to finish a project. **It is to become a better data scientist, with the emphasis on *'science'*.**

# The 8-week roadmap

| Week | Focus | Required Evidence of Progress (Deliverables) |
|---|---|---|
| **1. Kickoff** | Project framing and charter, scope, and project management, GitHub workflow | Project Charter, Initialized GitHub Repository | 
| **2. Get into the Data** | Data acquisition and quality, finalized project scope and background, and preliminary EDA | Formal Analysis Plan with Background/Introduction that includes in Appendix: (1) a data-loading attempt with brief "barebones" EDA and (2) data inventory (Data Dictionary/Codebook)
| **3. Prepare Data & Prevent Leakage** | Data cleaning, preprocessing, feature engineering, & leakage prevention | Reproducible cleaning and preprocessing workflow (repo) and Data Preprocessing & Leakage Prevention Report |
| **4. Polished EDA and Unsupervised Model(s)** | Report-ready EDA section and explore the utility of at least one unsupervised analysis | EDA and Unsupervised Model(s) Report |
| **5. Baseline Model(s)** | Fit the simplest appropriate baseline model(s) with evaluation and, **as appropriate**, interpretation | Baseline Model(s) Report |
| **6. Model Selection, Comparison, & Tuning** | Comparison of more complex models with baseline, including evaluation and tuning | (informal) Model Selection Report |
| **7. Final Model Selection** | Final model selection, validation, limitations, and interpretation | (informal) Final Model Report | 
| **8. Final Deliverables** | Communication and Portfolio completion | Final Technical Report, Reproducible GitHub repository |

## Week 1. Kickoff

### Focus:
To establish a shared understanding of the problem, explain why it matters, and plan how you will investigate it. Our goal is to provide stakeholders with the problem context, rationale, scope, and intended value.

### Milestone:
A clear project framing, a project charter, and an established project workspace (GitHub repo)

### Key Deliverable(s):

1. **Project Charter** document

2. **Project Repo** on GitHub

### You will be working toward...
- Project background and rationale
- A formal analysis plan, including the proposed data preparation, modeling, evaluation, interpretation, and communication approaches
- A project GitHub repository with an established workflow for organizing code, documentation, and tasks
- Beginning an approved data acquisition process

### Learning expectations:
Your project charter establishes a clear scope for your project (what it will and won't accomplish/answer) and gets your dataset approved. You will be learning how to write or contribute to project charters, as well as learning or improving your knowledge about how to manage and contribute to a GitHub repository. 

## Week 2. Get into the Data

### Focus:
To confirm that the project is feasible and begin learning what the data can and cannot tell you. You will also provide the broader project team / stakeholders with a feasible, data-informed analysis plan, evidence of engagement with the data, and any identified data-quality issues or risks.

### Milestone
An initial data inventory and EDA, with a confirmed project scope and final analysis plan

### Key Deliverable(s):

1. **Analysis Plan**, complete with:
  
  - Well-informed **background/introduction** to the problem
  
  - **Appendix** that contains:
  
    - "Barebones" initial exploratory data analysis (EDA)
    
    - Data inventory as a Data Dictionary or Codebook

### You will be working toward...
- Demonstrating the data you have obtained is feasible by showing concrete progress
- Identifying the unit of analysis, important variables, outcome or target where applicable, and relevant data limitations
- Beginning data quality checks and exploratory data analysis (EDA)
- Finalize the project scope and revise the analysis plan in light of what you have learned
- Identifying key steps for data cleaning and preprocessing, including challenges or barriers

### Learning expectations:
You are expected to continue to refine your GitHub skills, if needed, as well as to learn about your data, including the structure, fields, and data collection methods. You will need to be able to communicate limitations and risks to what the data can and cannot address relative to the question you presented in your charter. Further, you may need to learn about more sophisticated preprocessing or data leakage steps in anticipation of the next milestone and relative to what you learn about your data and the challenges it might present. 

**Note about data access:** 
Projects involving scraping or other data development may need additional time to fully meet this deliverable. If you anticipate a delay, request approval for an extension and show your progress, remaining steps, and fallback plan. An approved extension may provide up to one additional week for this milestone; it does not remove the need to make **timely** progress on the project.

**A final note about Analysis Plans**: 
An Analysis Plan is a starting point, not a promise that every method will work. You will refine it as you learn more about the data and receive feedback.

## Week 3. Prepare Data & Prevent Leakage

### Focus:
To build a defensible, reproducible workflow for preparing data for analysis and modeling, including appropriate barriers to data leakage or acknowledgements when control is likely to be insufficient.

### Milestone
A reproducible preprocessing workflow and a defensible evaluation setup complete with sufficient data leakage prevention

### Key Deliverable(s):
1. Data Preprocessing & Leakage Prevention Report

### You will be working toward...
- Addressing relevant data quality issues & finalizing data cleaning
- Developing preprocessing and data leakage prevention steps appropriate to the problem
- Deciding how to partition the data and validate the analysis
- Checking for potential leakage and other threats to valid evaluation
- Documenting important data preparation decisions
- Preparing for polished exploratory data analysis and unsupervised analyses

### Learning expectations:
Preprocessing choices depend on the data and the analytical task. Use the course materials and feedback to justify your choices rather than applying transformations mechanically or based on previous coursework or "standard" practices. You will be assessed on your **critical application** of preprocessing and data leakage prevention choices, meaning that your choices must be defensible. 

## Week 4. Polished EDA and Unsupervised Model(s)

### Focus:
To develop a deeper understanding of the prepared data, communicate the most meaningful patterns through a polished exploratory data analysis (EDA), and investigate whether unsupervised methods reveal useful structure in the data.

### Milestone
A report-ready EDA section and a documented assessment of the utility of appropriate unsupervised analysis.

### Key Deliverable(s):
1. **EDA and Unsupervised Model(s) Report**

### You will be working toward...
- Revisiting your preliminary EDA in light of what you learned during data preparation
- Identifying and communicating meaningful distributions, relationships, patterns, and limitations in the data
- Creating clear, well-labeled visualizations and interpreting their relevance to the project question
- Investigating whether appropriate unsupervised methods can reveal meaningful structure, subgroups, or lower-dimensional representations in the data
- Evaluating and interpreting unsupervised results where applicable, including relevant assumptions and limitations
- Refining feature engineering or other data preparation decisions when exploratory findings justify doing so
- Identifying findings that may inform subsequent model development and evaluation

### Learning expectations:
EDA is an iterative process. Your preliminary or "barebones" EDA helped you understand what data you had and identify potential problems; this milestone asks you to develop a more deliberate, coherent analysis that can be incorporated into your final technical report. You should select and interpret visualizations based on what they help you understand, not simply include every plot you produce.

Not every project will benefit from the same unsupervised methods, and you should not apply a technique simply because it is available. Choose an approach appropriate to your data and project goals, or explain why a particular type of unsupervised analysis is not useful or feasible. Your conclusions should reflect what the data and method can reasonably support.

Your EDA and unsupervised analyses should follow a defensible, reproducible workflow and respect the appropriate data partitions established for model evaluation. Document consequential changes to your preparation or analysis plan as your understanding of the data develops.


## Week 5. Baseline Model(s)

### Focus:
To establish meaningful reference points for evaluating predictive performance or other analytical approaches before investing in more complex models.

### Milestone
One or more defensible baseline approaches with initial evaluation results and documented modeling decisions, which includes an assessment of model assumptions.

### Key Deliverable(s):
1. **Baseline Model(s) Report**

### You will be working toward...
- Selecting and justifying an appropriate baseline for your analytical task
- Fitting a simple, meaningful model or analytical approach that provides a reference point for subsequent comparisons
- Establishing an evaluation strategy and selecting metrics appropriate to the problem
- Evaluating baseline performance using an appropriate validation approach
- Comparing results with a naive or other simple benchmark where appropriate
- Examining initial model behavior, errors, and limitations
- Documenting the baseline workflow, results, and decisions in your project repository
- Identifying potential improvements to investigate during model selection and comparison

### Learning expectations:
A baseline is not simply the first model that runs. It should provide a meaningful reference against which alternative approaches can be evaluated. The appropriate baseline depends on the task, the data, and the intended use of the results; for some projects, a simple statistical or rule-based approach may be more informative than a complex machine-learning model.

Your evaluation strategy should be appropriate to the data structure and intended use of the model. Use the validation approach established during data preparation, and ensure that comparisons are fair and that information from holdout test data does not influence model development. **You are not expected to optimize the baseline extensively at this stage.** The goal is to establish a credible starting point and understand what it tells you about the problem. However, you may want to start exploring options for next steps based on findings.


## Week 6. Model Selection, Comparison, & Tuning

### Focus:
To investigate whether alternative modeling approaches improve on the baseline and identify a defensible candidate for final evaluation.

### Milestone
A documented comparison of the baseline and appropriate candidate approaches, with preliminary results and a justified direction for final model selection.

### Key Deliverable(s):
1. (informal) **Model Selection Report**

### You will be working toward...
- Identifying candidate models or analytical approaches that are appropriate to the problem and informed by the baseline results
- Fitting and comparing candidate approaches using a consistent evaluation strategy
- Tuning selected models when justified by the problem, available data, and initial results
- Evaluating relevant performance measures and examining trade-offs between candidate approaches
- Investigating model behavior, errors, and potential weaknesses that may affect generalization
- Considering practical factors such as interpretability, computational cost, reproducibility, and potential deployment constraints
- Tracking experiments and documenting modeling decisions in your GitHub repository
- Identifying a preferred candidate and the remaining questions to address during final evaluation

### Learning expectations:
Model selection is a process of evaluating alternatives against the needs of the problem, not a competition to produce the most complicated model or the highest single performance score. There is also often a need to balance **interpretability by stakeholders** with complexity, so you will want to assess whether that balance impacts your project. Improvements should be supported by appropriate evaluation results, and differences in performance should be interpreted in light of the variability and limitations of the evaluation process.

Tuning should be purposeful and consistent with your evaluation strategy. Avoid repeatedly changing models without a clear rationale, and do not use the holdout test set to select features, tune hyperparameters, or choose a final model. By the end of this milestone, you should be able to explain which approach you currently favor, **why** you favor it, and what evidence is still needed before making a final recommendation to your broader project team and stakeholders.

**Important note**: Remember! More complex models are not automatically better. Your decisions should be supported by evaluation results and the needs of the problem, as well as balanced with any needs your stakeholders might have to understand or interpret the results. Also, do not move into tuning simply because it is the next step on the calendar. First establish that your baseline and evaluation process are meaningful and that tuning is a productive use of your effort and time.

## Week 7. Final Model Selection

### Focus:
To select and evaluate your final approach, interpret the results, and prepare the project for handoff or deployment. You will complete any remaining model comparisons and tuning of candidate models, clarify your tuning strategy, evaluate the results, identify limitations or remaining risks, and begin final wrap-up for your Final Deliverables in Week 8.

### Milestone
A final analysis with documented results, interpretation, limitations, and a clear path to reproducibility

### Key Deliverable(s):
1. (informal) Final Model Report

**Note**: This report is informal to give you more time for finishing the work rather than worrying about getting the writing down. Thus, only a brief report so that I can help advise on projects is required. 

### You will be working toward...
- Selecting a final model or analytical approach based on your evidence
- Completing appropriate validation and error analysis
- Interpreting the results in the context of the original problem
- Describing limitations and what should and should not be concluded, derived, used, deployed, or replicated from this work
- Checking that your repository and documentation allow another person to understand and reproduce your work

### Learning expectations:
Limitations can be introduced by the analysis, in addition to those introduced by the data collection method. Further, limitations will impact how users should interpret and apply model conclusions, so you will be expected to learn how to clearly communicate these limitations and any remaining risks with stakeholders and end-users of the data. Further, you will need to learn more about **deployability** of models, and decide whether (1) your model is deployable as-is and what method of deployment you suggest, (2) provide recommendations to get to deployment if your model is not ready yet, and (3) explain to users why your model failed if that is the end result. You invested time in trying to address this problem; if you decide it is not worth continuing, that is a valid recommendation to make **but** you need to be clear as to why you are making that recommendation and if anything could possibly salvage the project.


## Week 8. Final Deliverables

### Focus:
To communicate your work clearly and present a coherent, professional project. Your final work must includes final evaluation, interpretation, robustness, as well as an assessment of limitations and risks and a deployment plan (or why deployment is not advised).

### Milestone
A complete project package that communicates a defensible analysis and provides a reproducible record of the work

### Key Deliverable(s)

1. Final Technical Report

2. Polished GitHub Repo


### You will be working toward...
- Finalize the technical report and stakeholder-facing summary or presentation.
- Complete the GitHub README and organize code, documentation, and relevant outputs.
- Ensure that the repository explains the problem, data, methods, evaluation, results, limitations, and instructions for reproducing the analysis.
- Review the project against the course requirements and address remaining gaps.

**A note about "completion":** A successful Capstone is not defined by using the most complicated model or implementing every possible extension. It is defined by a clear problem, appropriate methods, credible evaluation, thoughtful interpretation, transparent limitations, and a professional, reproducible presentation of the work. Further, not every problem will make it to the same state of "doneness" because of challenges, barriers, or limitations in the dataset itself. As long as these are appropriately and thoroughly documented, there will be no penalty in the final deliverable. 

### Learning expectations:
You will learn how to communicate your findings to a mixed audience, both the intended stakeholder(s) as well as providing sufficient detail to satisfy other data scientists on your team or in your organization who may have questions about your methods, evaluation practices, or decision-making. Further, you will learn how to present a polished, well-organized repository as a portfolio to showcase your work as well as you ability to collaborate through remote repos and perform adqueate version control tracking with Git. 


# Working as a Data Science Team

The Capstone is both a technical project and an opportunity to practice professional project habits.

## Weekly standup discussion post

Each week, submit a standup discussion post addressing:

1. **Progress:** What did you complete since the previous update?
2. **Next steps:** What are your immediate priorities?
3. **Blockers:** What is uncertain, delayed, or preventing progress?
4. **Support needed:** What question or feedback would help you move forward?

These are discussion posts; **recording a video is optional**. Keep updates concise, specific, and useful to your teammates and instructor. Link to relevant GitHub issues, pull requests, code, or deliverables when appropriate.

## Collaboration and project management

Teams should make responsibilities visible, communicate when work is blocked, document important decisions, and keep project materials organized. Use the workflow and tools introduced in the course to help coordinate tasks and integrate work.

Team members should contribute meaningfully and understand the overall project, even when they take primary responsibility for different tasks. If your team encounters a workload or collaboration problem, raise it early rather than waiting until the final week.

Students approved to work individually are still expected to manage their work transparently, maintain an organized repository, communicate progress, and participate in applicable course feedback and peer-review activities.

# Your GitHub Portfolio

Your repository should evolve throughout the course. It is not something to assemble from scratch in Week 8.

By the end of Capstone, aim to include the following, as applicable to your project:

- **README:** Problem, context, objectives, project organization, key results, limitations, and reproduction instructions
- **Background and rationale:** Why the problem matters and what the analysis is intended to address
- **Analysis plan:** Intended approach and documented revisions as your understanding develops
- **Code and workflow:** Organized, readable scripts or notebooks, with clear instructions
- **Data documentation:** Data source, unit of analysis, variables, quality considerations, and access limitations. Do not publish confidential or restricted data
- **Results:** Relevant tables, figures, metrics, and model comparisons
- **Interpretation and limitations:** What the results mean, what they do not establish, and what further work may be needed
- **Reproducibility:** Dependencies, setup instructions, and steps another analyst would need to follow, subject to data-access restrictions

Your portfolio should show both the result and the reasoning behind it. A project with transparent decisions and credible limitations is stronger than one that reports impressive metrics without explaining how they were obtained.

I am not requiring that you organize your Portfolio in a specific way, but an example structure is given in the `README`.
