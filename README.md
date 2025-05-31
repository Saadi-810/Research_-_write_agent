# Research & Write Agent (CrewAI Project)

This project uses CrewAI to create a team of AI agents (Planner, Writer, and Editor) to generate blog posts or articles on a given topic. The agents collaborate to plan, write, and edit the content.

## Description

The `Research_&_write_agent.ipynb` notebook demonstrates how to set up and run a CrewAI-powered system. It defines three agents:
*   **Content Planner**: Plans engaging and fact-based content.
*   **Content Writer**: Writes a meaningful and fact-based opinion piece based on the planner's outline.
*   **Content Editor**: Edits the blog post to align with organizational style and journalistic best practices.

The notebook then defines tasks for planning, writing, and editing, and runs the crew to generate content on a specified topic (e.g., "Pakistan Vs India").

## Getting Started

### Prerequisites

Ensure you have Python installed. You will also need the `crewai` and `crewai_tools` libraries.

You will also need a Mistral API key. The notebook is configured to use Mistral models.
Set the following environment variables:
*   `OPENAI_API_KEY`: Your Mistral API key.
*   `OPENAI_API_BASE`: "https://api.mistral.ai/v1"
*   `OPENAI_MODEL_NAME`: e.g., "mistral-small"

You can install the required Python libraries using pip:
```bash
pip install -r requirements.txt
```

### Installation

1.  Clone the repo:
    ```sh
    https://github.com/Saadi-810/Research_-_write_agent.git
    ```
2.  Navigate to the project directory:
    ```sh
    cd Research_&_write_agent
    ```
3.  Set up your Mistral API key as an environment variable or directly in the notebook (as shown in the example, though using environment variables is recommended for security).

## Usage

1.  Ensure your environment variables for the Mistral API are set.
2.  Open the Jupyter Notebook:
    ```sh
    jupyter notebook Research_&_write_agent.ipynb
    ```
3.  Modify the `topic` variable in the `crew.kickoff()` input if you want to generate content on a different subject.
    ```python
    result = crew.kickoff(inputs={"topic":"Your New Topic Here"})
    ```
4.  Run the cells in the notebook sequentially to execute the agent crew and see the generated output. The final output is displayed using `IPython.display.Markdown`.

## Contributing

Contributions are welcome! If you'd like to contribute:
1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## License

This project is licensed under the MIT License - see the [`LICENSE`](LICENSE:0) file for details.

## Acknowledgments

*   This project is built using the [CrewAI](https://www.crewai.com/) framework.
