# Sion Park

AI engineer working on model development, evaluation, and deployment, with a background in Python backend and full-stack web services.

I work on edge AI systems: choosing models from measured data, validating them against clear evaluation criteria, and deploying them safely on real devices. I also build and operate web services end to end, including the backend, database, AI integrations, and deployment.

Outside my main field, I built [tourney-method](https://tourneymethod.com/), an osu! tournament archive and community contribution platform. I had no PHP or Laravel experience, so I used AI coding agents and documentation to learn the stack, build the service, and operate it as a public service. It shows that I can take on a domain I do not know yet and still deliver.

[GitHub](https://github.com/sionpkr) | [LinkedIn](https://www.linkedin.com/in/sion-park-4717602a6/) | [Email](mailto:pso9809@gmail.com)

## What I bring

- I work effectively in domains I do not know yet: I understand the service flow first, then use documentation, existing code, and AI tools, and I keep responsibility for direction, review, and validation.
- I turn a solved problem into reusable structure, so the next project does not start from zero.
- I take work from design through deployment and maintenance, and I state clearly what has and has not been measured.

## AI and MLOps

- **Model development:** Python, PyTorch, and scikit-learn. I compare candidate models under the same protocol, split data by test or event to avoid leakage, and choose with recall and false-alarm numbers.
- **Evaluation:** I prefer measured data over synthetic data, check per-group results and calibration, and record the limits next to the results.
- **Deployment:** ONNX and Hailo on Raspberry Pi, systemd services, signed releases, rollback, and human-approved promotion of models.
- **Practice:** test-driven development, evaluation gates before release, reusable project templates, and written decisions.
- **Tools:** I use AI coding agents such as Claude Code, review their work, and keep responsibility for validation.

## Skills

Operating systems

![OS](https://skillicons.dev/icons?i=linux,windows,raspberrypi)

Languages

![Languages](https://skillicons.dev/icons?i=python,php,typescript,javascript,c,cpp)

AI and data

![AI](https://skillicons.dev/icons?i=pytorch,sklearn,tensorflow,opencv)

Frameworks

![Frameworks](https://skillicons.dev/icons?i=django,flask,laravel,nextjs,react,tailwind)

Development environments

![IDE](https://skillicons.dev/icons?i=vscode,visualstudio)

Databases and tools

![Others](https://skillicons.dev/icons?i=mysql,postgres,mongodb,redis,docker,aws,githubactions,git,nginx)

## Featured projects

### [tourney-method](https://github.com/sionpkr/tourney-method)

A live platform for finding osu! tournaments, browsing tournament history, and contributing community records.

This is outside my main field of AI and machine learning. I took it on to show that, with AI coding agents and documentation, I can apply myself to areas I do not know well and still build and run something real.

- Built and operate [tourneymethod.com](https://tourneymethod.com/), with 1,000 logged-in users and active use in the osu! community.
- Started with no PHP or Laravel experience and used AI coding agents and documentation to build a production service in that stack.
- Plan the features, choose the technical approach, and design how community members contribute.
- Support tournament discovery, player and staff history, participation records, metadata corrections, multiple languages, and notifications.
- Maintain queue monitoring, backups, and health checks.
- Use AI coding agents to help with implementation, while taking responsibility for technical direction, code review, integration, and validation.

Built with Laravel 12, PostgreSQL, Redis, Livewire, Alpine.js, Tailwind CSS, Docker Compose, and Railway. Development tools include Pest, PHPStan, and Pint.

Community translations live in [tourney-method-locales](https://github.com/sionpkr/tourney-method-locales).

### [AICI / KT AIVLE School VOC TM](https://github.com/sionpkr/AICI_WEB)

A Django service for managing customer service (VOC) TM results and external construction reports, built during a company collaboration at KT AIVLE School.

- Led backend development and database design.
- Built authentication, role-based access control, construction and TM response status tracking, notices, and map-based construction information.
- Integrated AI models for speech-to-text, summarization, issue resolution detection, text correction, date and number formatting, and keyword extraction.
- Used my CS/VOC domain knowledge to clarify service workflows, establish shared terminology, and help the team decide what to build.
- Helped coordinate Git collaboration during backend and frontend integration. The team made over 200 commits in about two weeks.
- Received the Top Award among 50 participating teams.

### [Alyac Search / alyac_detect](https://github.com/sionpkr/alyac_detect)

A Python backend prototype for identifying pills from images and text.

- Built an API that reads text from uploaded images and returns matching pill data as JSON.
- Used Flask, a REST API, OCR, OpenCV-style image preprocessing, and public pill data.
- Filtered relevant object contours before inference to reduce unnecessary model work.
- Reported an 89.5% improvement in model processing speed through preprocessing and filtering.

## Tech stack

- AI and data: Python, PyTorch, scikit-learn, TensorFlow, ONNX, MLflow, Hailo, OpenCV, pandas, SQL, machine learning, deep learning, computer vision, NLP, web crawling, Roboflow
- Backend: Python, Django, Flask, REST API, PHP, Laravel, MySQL, PostgreSQL, MongoDB
- Frontend and apps: JavaScript, TypeScript, Next.js, HTML, CSS, React Native, Livewire, Alpine.js, Tailwind CSS, PyQt5
- Infrastructure and development: Linux, systemd, Docker, Docker Compose, Git, GitHub, GitHub Actions, AWS, Gunicorn, Nginx, Redis, Railway, Vite, pytest, Pest, PHPStan, Pint

## How I work

I learn unfamiliar domains through documentation, existing code, and conversations with users and communities. I turn that understanding into specifications, flowcharts, and shared terminology so the team can agree on what to build.

I like taking a service through design and implementation to deployment and maintenance, including AI integration when the project calls for it. I use spec-driven development and AI coding agents, and take responsibility for reviewing and integrating the results.

I keep decisions and implementation notes in writing, using Git and issue-style planning to make the work easier to follow.

## Current focus

I'm focused on edge AI model development and deployment: building the evaluation and release practices around the models, and measuring before optimizing. I keep operating tourney-method in production while deepening my Python, PyTorch, and Linux deployment skills. I'm also refining how I use AI coding agents, particularly how I write specifications, review their work, and validate changes.
