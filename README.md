# Sion Park

AI engineer working on the evaluation, approval, and deployment side of edge AI (MLOps), with a background in Python backend and full-stack web services.

At work I built an internal MLOps library and project template for sensor AI projects, which is now applied to two ongoing edge AI projects. I also build and operate web services end to end, including the backend, database, AI integrations, and deployment.

Outside my main field, I built [tourney-method](https://tourneymethod.com/), an osu! tournament archive and community contribution platform. I had no PHP or Laravel experience when I started, so I learned the stack from documentation and AI coding agents, then built the service and now run it publicly.

[GitHub](https://github.com/sionpkr) | [LinkedIn](https://www.linkedin.com/in/sion-park-4717602a6/) | [Email](mailto:pso9809@gmail.com)

## What I bring

- In a domain I do not know yet, I start from the service flow and use documentation, existing code, and AI tools, while I stay responsible for direction, review, and validation.
- A problem I have solved once becomes reusable structure, so the next project does not start from zero. The internal MLOps library started that way, on my own initiative.
- I take work from design through deployment and maintenance, and I say what has and has not been measured.

## AI and MLOps

I work in Python with PyTorch and scikit-learn. Candidate models run under the same protocol, data is split by test or event to avoid leakage, and I choose models from measured data and write the limits next to the results.

For deployment I use ONNX and Hailo-8, systemd services, Ed25519-signed release bundles, atomic install with automatic restore after a failed switch, manual rollback, and human-approved model promotion. Around that sit test-driven development, evaluation gates before release, reusable project templates whose improvements reach existing projects through `copier update`, and written decisions. Rollback covers install and switch failures. Model-quality monitoring and automatic retraining are not part of my experience yet.

I use AI coding agents (Claude Code, Codex, GLM) and read-only reviewer agents, and I adopt a change only after the tests and the review agree.

## Skills

Operating systems

![OS](https://skillicons.dev/icons?i=linux,windows)

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

### enitt_mlops (internal work project, private repository)

An MLOps library and `copier` project template for sensor AI projects.

- Started on my own after seeing data contracts, signed deployment, evaluation gates, and edge installers rebuilt for each project.
- A core that knows nothing about the sensor, plus sensor plugins loaded through entry points. A plugin that fails to load does not stop the core CLI.
- Release bundles are Ed25519-signed and hash-checked. The edge installer installs atomically, restores the previous state when the post-switch check fails, and supports manual rollback. Edge packages run without mlflow, torch, or pandas, enforced by import tests.
- The evaluation gate accepts only group-wise cross-validation results, checks sample-size minimums and regression against the current model, and blocks promotion if any check fails. A person approves promotion.
- About 16k lines of tests, including template tests that generate a project, install it, and run its tests.
- Status: started in November 2026 and applied to two ongoing edge AI projects. There are no long-term operating results yet.

### [tourney-method](https://github.com/sionpkr/tourney-method)

A live platform for finding osu! tournaments, browsing tournament history, and contributing community records.

This is outside my main field of AI and machine learning. I built it with AI coding agents and documentation, in a stack I had not used before.

- Built and operate [tourneymethod.com](https://tourneymethod.com/). It had its first public release in May 2026, and more than 1,700 accounts have logged in (cumulative, as of November 2026).
- Plan the features, choose the technical approach, and design how community members contribute.
- Support tournament discovery, player and staff history, participation records, metadata corrections, multiple languages, and notifications.
- Maintain queue monitoring, backups, and health checks. A daily job reads osu! forum posts into the database with one job per post, retries, and duplicate protection. A backup runs before data changes, and the restore path is tested.
- Use AI coding agents to help with implementation, while taking responsibility for technical direction, code review, integration, and validation.

Built with Laravel 12, PostgreSQL, Redis, Livewire, Alpine.js, Tailwind CSS, Docker Compose, and Railway. Development tools include Pest, PHPStan, and Pint.

Community translations live in [tourney-method-locales](https://github.com/sionpkr/tourney-method-locales).

### [AICI / KT AIVLE School VOC TM](https://github.com/sionpkr/AICI_WEB)

A Django service for managing customer service (VOC) TM results and external construction reports, built during a company collaboration at KT AIVLE School.

- Owned the Django backend, the database structure design, and security checks.
- Built authentication, role-based access control, construction and TM response status tracking, notices, and map-based construction information.
- Integrated AI models for speech-to-text, summarization, issue resolution detection, text correction, date and number formatting, and keyword extraction.
- Used my CS/VOC domain knowledge to clarify service workflows, establish shared terminology, and help the team decide what to build.
- Helped coordinate Git collaboration during backend and frontend integration. The team made over 200 commits in about two weeks.
- Received the Top Award among 50 participating teams.

### [Alyac Search / alyac_detect](https://github.com/sionpkr/alyac_detect)

A Python backend prototype for identifying pills from images and text.

- Built an API that reads text from uploaded images and returns matching pill data as JSON.
- Used Flask with flask-restx for the REST API, EasyOCR for text recognition, and a public pill dataset.
- Filtered relevant object contours before inference to reduce unnecessary model work.
- Preprocessing and contour filtering cut model processing time by 89.5% compared with feeding the original image (measured at the time; the measurement setup was not recorded).

## Tech stack

- AI and data: Python, PyTorch, scikit-learn, TensorFlow, ONNX, MLflow, Hailo, OpenCV, pandas, SQL, machine learning, deep learning, computer vision, NLP, web crawling, Roboflow
- Backend: Python, Django, Flask, REST API, PHP, Laravel, MySQL, PostgreSQL, MongoDB
- Frontend and apps: JavaScript, TypeScript, Next.js, HTML, CSS, React Native, Livewire, Alpine.js, Tailwind CSS, PyQt5
- Infrastructure and development: Linux, systemd, Docker, Docker Compose, Git, GitHub, GitHub Actions, AWS, Gunicorn, Nginx, Redis, Railway, Vite, pytest, Pest, PHPStan, Pint

## How I work

I also learn from conversations with users and communities, and I turn that understanding into specifications, flowcharts, and shared terminology so the team can agree on what to build. I use spec-driven development (Spec Kit) and AI coding agents, and I review and integrate the results myself. On tourney-method I first planned with BMAD Method, restarted from scratch when the stories did not connect in implementation, and moved to Spec Kit with maintained documents, so a new AI session can continue from the previous session's progress.

I keep decisions and implementation notes in writing, using Git and issue-style planning to make the work easier to follow.

## Current focus

I'm focused on MLOps for edge AI: the evaluation, approval, signed deployment, and rollback practices around the models, and measuring before optimizing. I keep operating tourney-method in production while deepening my Python, PyTorch, and Linux deployment skills. I'm also refining how I use AI coding agents, particularly how I write specifications, review their work, and validate changes.
