Note: This is a very summarized version of the research paper "[Designing for Cognitive Diversity: Improving the GitHub Experience for Newcomers](https://github.com/streats/a11y-champions/blob/main/github-gender-inclusivity-bugs.md)", intended primarily for the benefit of neurodiverse people and anyone who is unable (or unwilling!) to read the full report. Please note this summary was generated using ChatGPT and therefore may skim over some important nuances or caveats. Detailed data, links, and citations/references have been excluded and can be found in the full report. 

# Summary - Designing for Cognitive Diversity: Improving the GitHub Experience for Newcomers

## Introduction
- The study addresses cognitive style bias on platforms like GitHub.
- GenderMag was used to identify inclusivity issues.
- A browser plugin was developed to redesign problematic features.
- Testing with 75 participants showed improved user performance, especially for those with cognitive styles linked to women.
- The study emphasizes accommodating cognitive diversity in software design for inclusivity.
- It explores the role of Open Source Software (OSS) projects in workforce development and inclusion.
- Challenges faced by newcomers, especially those with unsupported cognitive styles, are highlighted.
- The study aims to reduce cognitive barriers and promote diversity in the OSS community.

## Related Work
- Previous research has extensively investigated the challenges faced by newcomers when contributing to Open Source Software (OSS) projects, identifying numerous barriers and obstacles.

- Toxic environments within OSS communities, characterized by unfriendly, unhelpful, or elitist behaviors among project members, have been a subject of study.

- Research has delved into the response times and types of responses that newcomers receive, considering factors like gender and nationality.

- Concerns regarding the lack of diversity in OSS communities have been raised, spanning gender, language, and location diversity. Studies have shown that diverse teams tend to be more productive, but underrepresented groups face difficulties integrating into OSS communities.

- The prevalent meritocratic nature of OSS communities has been criticized for fostering imposter syndrome and discouraging participation from minorities, particularly women.

- Observations in OSS contributions have revealed that men tend to dominate code authorship while undermining the social ties necessary for women's inclusion.

- Studies have also highlighted the existence of distinct cognitive styles and motivations among developers, with women often displaying task-oriented tendencies and men being more motivated by the enjoyment of learning new technologies.

- These cognitive style differences can significantly affect how individuals, especially women, contribute to OSS projects, particularly when project structures favor specific cognitive styles over others.

- The study's primary goal is to address these issues by proposing modifications to GitHub to make it more inclusive and supportive of newcomers with diverse cognitive styles.


## Research method
The study followed a three-step process:

1. **Identifying GitHub Inclusivity Bugs**: They used the GenderMag method, which assesses software for gender-related biases by considering cognitive styles. This method uses personas (Abi, Pat, Tim) representing different cognitive styles based on five facets: motivation, information processing styles, computer self-efficacy, risk aversion, and learning style. Inclusivity bugs are identified when these personas face difficulties during a use case evaluation.

2. **Fixing GitHub Inclusivity Bugs**: Proposed fixes to address the inclusivity bugs identified in GitHub, then developed a browser plugin to implement these changes in the GitHub interface.

3. **Assessing Inclusivity Bugs Fixes**: Conducted an experiment to compare the original GitHub interface with the modified interface enriched by the plugin. 


### Step 1 - Identify

- GenderMag method evaluates software for inclusivity bugs based on cognitive styles.
- Three personas used: Abi, Pat, Tim, representing different cognitive facets.
- Five facets considered: motivation, information processing styles, computer self-efficacy, risk aversion, learning style.
- Negative answers related to cognitive styles indicate inclusivity bugs.
- Study focuses on Abi and Tim personas customized for GitHub newcomers.
- Four use cases evaluated: editing a file, submitting a pull request, forking a repository, uploading a new file.
- Six researchers identified 12 inclusivity bugs in GitHub's interface.

### Step 2 - Fix 

- GitHub interface redesigned based on GenderMag analysis to address inclusivity issues.
- GenderMag analysis identifies inclusivity bugs and underlying facets contributing to issues.
- Example: UC#1 revealed Abi's process-oriented learning style and self-efficacy issues.
- Redesign solutions focused on enhancing visibility and guidance.
- A Chrome extension plugin developed to implement interface modifications.
- Plugin collects user data in JSON format and is publicly available on GitHub.

### Step 3 - Assess

In this experiment, researchers compared the impact of a modified GitHub interface (Plugin group) with the original interface (Control group) on users with different cognitive styles (Abi-like and Tim-like).

* **Participants**: 75 undergraduate students, mostly from computer science backgrounds, who knew how to program but had never opened a pull request on GitHub.

* **Method**: Participants completed four use cases in an open-source project named JabRef3. They assessed their confidence (self-efficacy) before and after the experiment. Qualitative data were collected about difficulties and interface aspects.

* **Findings**: The study aimed to reduce the performance gap between Abi-like and Tim-like users. The modified interface intended to improve effectiveness and self-efficacy for Abi-like users.

## Results

### Discovering and Fixing inclusivity bugs on GitHub
- Study identifies 12 inclusivity bugs in GitHub interface using GenderMag evaluation.
- Bugs mainly affect users with Abi-like cognitive traits.
- Fixes aim to enhance visibility, feedback, and reduce information overload.
- Enhancements include progress bars and tooltips.
- Focus is on improving the experience for GitHub newcomers.

  
### Effects of removing GitHub inclusivity bugs
- Study evaluates interface redesign impact on Abi and Tim participants in terms of completion rates and self-efficacy.
- UC#1 showed no significant difference, but Abis in the Plugin group performed slightly better.
- UC#2 and UC#3 had challenges for Abis in the Control group, while both Abis and Tims in the Plugin group had higher completion rates.
- UC#4 was challenging for all, but the redesign significantly improved completion rates for both Abis and Tims.
- Redesign also boosted participants' self-efficacy.
- Overall, GenderMag-inspired redesign reduces task completion gaps and enhances self-efficacy.

## Discussion

- Study focuses on GitHub's inclusivity bugs related to cognitive styles (Abis and Tims) and gender implications.
- Identifies 12 inclusivity bugs mainly affecting Abi-like users, addressing information processing, self-efficacy, and learning styles.
- Aligns with previous GenderMag research, highlighting similar barriers in open-source projects like inadequate information, low computer self-efficacy, and unclear instructions for process-oriented learners.
- Emphasizes fixing inclusivity bugs benefits not only Abi-like users but also the broader user base.
- Highlights the severe gender diversity gap in open-source communities and the importance of inclusivity for attracting newcomers and preventing demotivation, especially among students and novices.


## Implications

1. Social coding platforms need inclusive design considering diverse user cognitive styles.
2. Maintainers should address inclusivity bugs and provide clearer documentation.
3. Newcomers should understand interface challenges and respect cognitive style differences.
4. Educators should help students overcome GitHub challenges and explore better teaching methods.

## Limitations

1. Focusing on the Abi persona could leave other newcomers less supported, but our results show some improvements for all.
2. Gender imbalance in the sample despite recruitment efforts, impacting generalizability.
3. GenderMag analysis relies on gender but can address inclusivity without discussing gender.
4. Sample not representative, focused on initial evidence in a controlled environment.
5. Plugin behavior variation among browsers addressed with pre-configured computers.
6. Challenges in comparing task completion times due to a high number of non-completions.
7. Qualitative analysis conducted with two researchers to minimize subjectivity and enrich results.

## Conclusion

This study identifies 12 inclusivity bugs in GitHub's interface, primarily affecting users with cognitive styles common among women. They propose fixes, implement them as a plugin, and test them with 75 newcomers, resulting in significant usability and self-efficacy improvements. Future work aims to further address inclusivity barriers in tools and infrastructure for enhanced engagement in open-source projects.
