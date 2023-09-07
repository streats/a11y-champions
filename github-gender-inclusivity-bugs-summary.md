Note: This is a very summarized version of the research paper "[Designing for Cognitive Diversity: Improving the GitHub Experience for Newcomers](https://github.com/streats/a11y-champions/blob/main/github-gender-inclusivity-bugs.md)", intended primarily for the benefit of neurodiverse people and anyone who is unable (or unwilling!) to read the full report. Please note this summary was generated using ChatGPT and therefore may skim over some important nuances or caveats. Detailed data, links, and citations/references have been excluded and can be found in the full report. 

# Summary - Designing for Cognitive Diversity: Improving the GitHub Experience for Newcomers

## Introduction
This paper addresses cognitive style bias on social coding platforms, such as GitHub, which can hinder certain populations, particularly women. They used GenderMag to identify inclusivity issues, developed a browser plugin to redesign problematic features, and tested it with 75 participants. Results showed improved user performance and self-efficacy, especially for those with cognitive styles linked to women. This highlights the importance of accommodating cognitive diversity in software design for a more inclusive environment.

This study explores the significance of Open Source Software (OSS) projects in fostering workforce development and inclusion. It highlights challenges faced by newcomers, especially underrepresented groups with unsupported cognitive styles, which can impede diversity in OSS projects. The research focuses on identifying and addressing inclusivity bugs in GitHub, a popular OSS platform. Through interface redesign and a browser plugin, the study aims to reduce cognitive barriers for newcomers, ultimately promoting diversity and inclusion within the OSS community.

## Related Work
This section addresses challenges in newcomer onboarding to open-source software (OSS) projects, the lack of diversity and biases in OSS communities, and the impact of different cognitive styles on OSS contributions.

- **Newcomer Onboarding**: Previous research has identified barriers for newcomers in OSS, including unfriendly environments and slow responses. The study aims to enhance inclusivity on social coding platforms, focusing on accommodating various cognitive styles.

- **Diversity/Bias in OSS**: Concerns about diversity, including gender, language, and location diversity, exist in OSS communities. The study aims to reduce bias in social coding platforms, making them more inclusive for users with diverse cognitive styles.

- **Cognitive Styles**: Research highlights varying cognitive styles and motivations among software developers, which can influence OSS contributions. The study proposes GitHub changes to support a broader range of newcomers with different cognitive styles.

## Research method
The study followed a three-step process:

1. **Identifying GitHub Inclusivity Bugs**: They used the GenderMag method, which assesses software for gender-related biases by considering cognitive styles. This method uses personas (Abi, Pat, Tim) representing different cognitive styles based on five facets: motivation, information processing styles, computer self-efficacy, risk aversion, and learning style. Inclusivity bugs are identified when these personas face difficulties during a use case evaluation.

2. **Fixing GitHub Inclusivity Bugs**: Proposed fixes to address the inclusivity bugs identified in GitHub, then developed a browser plugin to implement these changes in the GitHub interface.

3. **Assessing Inclusivity Bugs Fixes**: Conducted an experiment to compare the original GitHub interface with the modified interface enriched by the plugin. 


### Step 1 - Identify

The study used GenderMag, a method for evaluating software for inclusivity bugs based on cognitive styles, which tend to cluster by gender. GenderMag employs personas (Abi, Pat, Tim) representing different cognitive facets. Five facets are considered:

1. **Motivation**: Abis focus on what they can accomplish with technology, while Tims are motivated by the enjoyment of technology itself.

2. **Information Processing Styles**: Abis gather complete information before proceeding, while Tims use selective information processing, following promising leads.

3. **Computer Self-Efficacy**: Abis have lower confidence in specific tasks compared to Tims, affecting their strategies and persistence.

4. **Risk Aversion**: Abis are more risk-averse when trying new features compared to Tims.

5. **Learning Style**: Abis prefer process-oriented learning, while Tims enjoy experimenting with new software features.

The GenderMag method involves evaluation teams using personas to assess software, answering questions related to subgoals and actions. Negative answers, particularly related to cognitive styles, indicate inclusivity bugs.

In this study, Abi and Tim personas were selected to represent opposite ends of the GenderMag facet ranges. They were customized to reflect newcomers wanting to make their first GitHub contribution. Four use cases were identified: editing a file, submitting a pull request, forking a repository, and uploading a new file.

Six researchers conducted GenderMag evaluations on GitHub-hosted projects for these personas. They identified 12 inclusivity bugs in various parts of the GitHub interface.

### Step 2 - Fix 

The GitHub interface was redesigned to address inclusivity issues related to the GenderMag facets identified in Step 1. GenderMag analysis not only identifies inclusivity bugs but also provides insights into why they occur and which facets are involved.

As an example, for Use Case #1 (UC#1), an issue related to Abi's process-oriented learning style and self-efficacy facets was identified, affecting her ability to edit a file in an OSS project. The redesign focused on Abi's process-oriented learning by enhancing visibility and guidance. This included presenting README file information more explicitly through a new "home" tab and adding a tooltip to explain the file editing process.

Once the research team agreed on the redesign solutions for each identified issue, they developed a Chrome extension plugin to modify GitHub's interface. This plugin, built in JavaScript and utilizing the GitHub API, collects user data in JSON format. It is publicly available on GitHub for use and contributions.

### Step 3 - Assess

In this experiment, researchers compared the impact of a modified GitHub interface (Plugin group) with the original interface (Control group) on users with different cognitive styles (Abi-like and Tim-like).

**Participants**: 75 undergraduate students, mostly from computer science backgrounds, who knew how to program but had never opened a pull request on GitHub.

**Method**: Participants completed four use cases in an open-source project named JabRef3. They assessed their confidence (self-efficacy) before and after the experiment. Qualitative data were collected about difficulties and interface aspects.

**Findings**: The study aimed to reduce the performance gap between Abi-like and Tim-like users. The modified interface intended to improve effectiveness and self-efficacy for Abi-like users.

## Results

### Discovering and Fixing inclusivity bugs on GitHub
The study identified 12 inclusivity bugs in the GitHub interface using the GenderMag evaluation method. These bugs affected users with different cognitive styles, particularly those with Abi-like traits. The fixes focused on improving visibility, feedback, and reducing information overload. For instance, a progress bar and tooltips were added to guide users through the process. The study aimed to enhance the user experience for newcomers trying to make their first contribution on GitHub.

### Effects of removing GitHub inclusivity bugs
The study evaluated the impact of their interface redesign on completion rates and self-efficacy of Abi and Tim participants. For UC#1, there was no significant difference between the groups, but Abis in the Plugin group performed slightly better. For UC#2 and UC#3, Abis in the Control group faced challenges, while both Abis and Tims in the Plugin group had higher completion rates. UC#4 was challenging for all, but the redesign significantly improved completion rates for both Abis and Tims. The redesign also improved participants' self-efficacy. Overall, the GenderMag-inspired redesign helped reduce task completion gaps and enhance self-efficacy.

## Discussion

This study examined inclusivity bugs in the GitHub interface, particularly how they affect users with different cognitive styles (Abis and Tims) and their gender implications. The research aligns with past findings that software often contains inclusivity bugs that disproportionately impact users with certain cognitive styles, potentially creating barriers to participation. The study identified 12 inclusivity bugs that predominantly affect Abi-like users, addressing issues related to information processing, self-efficacy, and learning styles.

The findings concur with previous GenderMag research, which identified similar facets as barriers to contributions in open-source software projects, including inadequate upfront information, low computer self-efficacy, and a lack of clear instructions for process-oriented learners. The study highlights that fixing these inclusivity bugs not only benefits Abi-like users but can also improve the software for the broader population, as shown in prior research.

Moreover, the study emphasizes the importance of inclusivity in open-source software tools and technology. It points out the severe gender diversity imbalance in open-source communities and highlights the need to make these environments more inclusive, as inclusivity bugs can contribute to feelings of not belonging and impostor syndrome among underrepresented groups. Ensuring that tools like GitHub accommodate diverse cognitive styles is crucial for attracting newcomers and preventing skill-related demotivation, particularly among students and individuals with limited experience.


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
