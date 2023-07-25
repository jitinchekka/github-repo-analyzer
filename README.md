# Github Automated Analysis Project
   The GitHub Repository Analyzer is a Python-based tool that helps you find the most technically complex and challenging repository from a GitHub user's profile. By utilizing advanced language models such as GPT and LangChain, the tool can assess each repository individually and make an informed decision about the repository's technical complexity.


## How It Works
The GitHub Repository Analyzer uses the following steps to determine the most technically challenging repository:

1. **Input**: Provide the GitHub user's URL as input to the tool.
2. **Fetch Repositories**: The tool will fetch all public repositories from the provided user's GitHub profile using the GitHub API.
3. **Assessment**: For each repository, the tool will utilize the power of GPT and LangChain to assess its technical complexity and challenges based on various factors such as code complexity, usage of advanced algorithms, number of contributions, pull requests, issues, and other relevant metrics.
4. **Scoring**: The tool will assign a score to each repository based on the assessment results.
5. **Selecting the Most Challenging Repository**: After analyzing all the repositories, the tool will identify and display the repository with the highest score as the most technically complex and challenging one.

It uses [Langchain](https://langchain.com/), OpenAI API (gpt-3.5-turbo model), and FAISS as vector store which efficient Prompt Engineering under the hood. It considers different factors for determining the most complex repository such as algorithmic complexity, code complexity, coupling and cohesion between classes and modules, cyclomatic complexity, number of contributions, pull requests, issues, and other relevant metrics.

## Demo
[Demo](https://jitin-git-repo.streamlit.app/)
## Getting Started

These instructions will help you set up the project and run it on your local machine.

### Prerequisites
```
- Install [Python](https://www.python.org/downloads/) 3.9.0 or later
- Set up a virtual environment (Optional but Recommended)
```

### Installation

1. Clone this repository to your local machine.
   ```
   git clone https://github.com/jitinchekka/github-repo-analyzer.git
   ```

2. Go to the project folder.
   ```
   cd github-repo-analyzer
   ```

3. Create a virtual environment.
   ```
   python -m venv venv
   ```

4. Activate the virtual environment.
   - On Windows:
       ```
       .\venv\Scripts\activate
       ```
   - On Linux or MacOS:
       ```
       source venv/bin/activate
       ```

5. Install the required dependencies using the following command.
   ```
   pip install -r requirements.txt
   ```

6. Create a `.env` file to store sensitive information (such as API keys or tokens) required for the GitHub API:
   ```
   touch .env
   ```
   Add your GitHub API token, OPENAI_API_KEY, ACTIVELOOP_TOKEN to the `.env` file in the following format:
   ```
   GITHUB_TOKEN="MY-TOKEN"
   OPENAI_API_KEY="MY-KEY"
   ACTIVELOOP_TOKEN="MY-TOKEN"
   ```

## Running the application

1. Run the streamlit application.
   ```
   streamlit run app.py
   ```

2. Open your web browser and enter the URL shown in the terminal, usually `http://localhost:8501`

3. Enter the GitHub username in the input box and click on the `Submit` button.

## Customization

The GitHub Repository Analyzer allows you to customize certain parameters to adjust the assessment process according to your requirements. You can find these parameters in the `config.py` file.

## Built With

- [Python](https://www.python.org/)
- [Streamlit](https://www.streamlit.io/)
- [LangChain](https://langchain.com/)
- [OpenAI API](https://platform.openai.com/docs/introduction)
- [FAISS](https://faiss.ai/index.html) 

## Contributing

Contributions to the GitHub Repository Analyzer are welcome! If you find any issues or have ideas for improvements, feel free to open an issue or submit a pull request. Please ensure that you adhere to the project's code of conduct.

## Acknowledgments

The GitHub Repository Analyzer was inspired by the Github Automated Analysis Project by Mercor. It utilizes the power of GPT and LangChain, both of which are incredible technologies.

## Contact

If you have any questions or need further assistance, please feel free to contact me at the following email address

- Jitin (jitinchekka2@gmail.com)

Happy analyzing and coding!


