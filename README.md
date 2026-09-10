# PromptMe - A Vulnerable LLM Application

<p>
<img src="https://github.com/R3dShad0w7/PromptMe/blob/main/static/logo.png?raw=true" width="600" alt="Thumbnail"/>
</p>

### A vulnerable application designed to demonstrate the OWASP Top 10 for Large Language Model (LLM) Applications.

PromptMe is an educational project that showcases security vulnerabilities in large language models (LLMs) and their web integrations. It includes 10 hands-on challenges inspired by the OWASP LLM Top 10, demonstrating how these vulnerabilities can be discovered and exploited in real-world scenarios.

This project is intended for AI Security professionals to explore potential security risks in LLMs and learn effective mitigation strategies.

## Overview (No API Key required)

The project is primarily developed using Python and the Ollama framework, with the open source LLM models. The exercises are structured in the form of **CTF (Capture The Flag) challenges**, each with a clear objective, optional hints, and a flag awarded upon successful completion.

## Gettting started

This guide provides instructions for setting up and running the challenges.

### Prerequisites

* Python 3.10 or higher
* pip (Python package installer)
* ollama framework 

### Setup

#### 1. Clone the repository.
> ```
> git clone https://github.com/R3dShad0w7/PromptMe.git
> ```

#### 2. Go to challenge directory.
> ```
> cd PromptMe
> ```

#### 3. Install the dependencies.
> ```
> pip install -r requirements.txt
> ```

#### 4. Download and Run Ollama

> Download Ollama depending on your OS from https://ollama.com/download
>```
> ollama serve (in the separate terminal)
> ollama pull mistral
> ollama pull llama3
> ollama pull sqlcoder
> ollama pull granite3.1-moe:1b
> ollama pull granite3-guardian
>```
>or Spawn Ollama via docker using the below command
> ```
> docker run -d --name ollama_server -p 11434:11434 ollama/ollama:latest
> docker exec -it ollama_server ollama pull <model_name>
> docker exec -it ollama_server ollama run <model_name>
> ```

#### 5. Access the application

> ```
> python main.py
> ```
Access the application @ http://127.0.0.1:5000

#### 6. Start the challenge by clicking *start* button on particular category e.g. LLM01

## Compatibility 

This project currently supports macOS and Linux systems. Windows compatibility is in progress and will be released in an upcoming update.

## Spoilers

[Solutions](https://github.com/R3dShad0w7/PromptMe/tree/main/solutions) to the challenges are provided for beginners who may not be familiar with exploiting vulnerabilities from the LLM Top 10. This guide is intended to help users solve the challenges and understand the underlying vulnerable code and components.

## Connect

If you face any challenges in setup, solving or any suggestions, please reach out to https://discord.gg/CYnjfxNhgU


## Disclaimer

PromptMe is an intentionally vulnerable application created for educational purposes. Since the application uses insecure code and packages to demonstrate possible risks, it is strongly recommended to run it in a virtual or sandboxed environment.
Warning: The vulnerabilities shown in this project are for learning only and should never be implemented in production systems.

🤝 Contributing

We welcome contributions from the community! Whether you're fixing bugs, improving documentation, or suggesting new challenges, your help is appreciated.

If you're interested in contributing:

    Fork the repository.

    Create a new branch (git checkout -b feature-name).

    Make your changes and commit them.

    Push to your fork and create a Pull Request.


## License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/R3dShad0w7/PromptMe/blob/main/LICENSE) file for details.

## Author

The project is developed and maintained by [Divyesh](https://github.com/divyesh-0x01), [Srithesh](https://github.com/0xbughunter), [Praveen](https://github.com/praveen-kv), [Ranjit](https://www.linkedin.com/in/ranjit-singh-a788b579/), [Sumanth](https://github.com/SumanthGowda)
