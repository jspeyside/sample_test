node {
    stage 'Install Dependencies'
    env.WORKSPACE = pwd()
    sh 'virtualenv venv'
    sh '. venv/bin/activate'
    sh '${env.WORKSPACE}/venv/bin/pip install -r requirements.txt'

    stage 'Test'
    sh '${env.WORKSPACE}/venv/bin/python install runtests.py'
}
