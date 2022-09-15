@Library('jenkins-pipeline-library@v8')

def pipeline_vars = [
    // required
    SERVICE_NAME: "nhgis-assets",
    BRANCH_NAME: env.BRANCH_NAME,
    verify_endpoint: "/",
    verify_method: "GET",
    verify_expected_code: "200",
    ALLOW_OUTSIDE_ACCESS: true,

    // optional
    TEST_COMMAND: "echo",
    HOST: "assets.nhgis.org",
    THIS_API_SERVER: "assets.nhgis.org",
    MAX_START_RETRIES: 8,
    START_RETRY_WAIT: 3,
]

apiDeliveryPipeline(pipeline_vars)