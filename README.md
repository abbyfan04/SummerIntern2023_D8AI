# SummerIntern2023_D8AI

D8AI(https://d8ai.com/) is an AI solution provider in Taiwan that provides businesses with custom chatbots. As an intern in the R&D department, I developed 2 APIs for D8AI, aiming to improve their client's experience in producing a chatbot. By creating the two programs, D8AI and its clients would no longer need to spend time coming up with questions one by one. Now, the program would provide a first draft, and workers would only need to make changes to the original document. While D8AI mainly supports local middle to small businesses in Taiwan, the product was prompted based on Traditional Mandarin. Therefore, comments in English and Mandarin are added in order to easier understanding of the code.

## Description

The file, _Initial_Generation_1Q1A_問題集從無到有_API_ver_, is the initial generation of question-and-answer sets from quantitative data provided by the client, usually in PDF format. The pdf would include most if not everything they want the custom robot to answer, including contents from official websites, workers' manuals, and personal experience. After running the API, an Excel of QA sets with 1Q to 1A would be created.

The other file, _chatgpt_1q_to_multiple_q-11_API_ver_, is a program that could be used after the generation of the 1Q1A dataset to improve its performance. In this program, number of questions linking to an answer would be increased. The number of questions would be increased based on two factors. First, if there are any parts or keywords included in the answer that the existing question fails to cover, the program will come up with additional questions. Secondly, if there are no additional questions that could be made based on content, more questions would be generated based on semantics. In this case, questions that have the same meaning but with different grammatical structures would be generated.

## Getting Started

### Dependencies

* OpenAI Developer account: As the programs implemented chat3.5 from OpenAI, a secured API key would be needed.
* Traditional Chinese Dataset Only: As the program is specifically prompted for Taiwanese businesses, the prompt is based on the language most commonly used there.

## Authors

* Abby Fan: abby040325@gmail.com
