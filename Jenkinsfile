@Library('IDAPPipelineCommon')
@Library('IDAPPipelineConfig')


def pipeline = pipelineManager.config()

def buildType = new com.corelogic.pipeline.DeployableType(
        appName: 'helloworld',
        ecosystemName:'NASPipeline',
        deployToCF: true,
        pipelineFlowName: 'normalFlow'
)

pipeline.getConfig().setNode('edgeportals')
pipeline.getConfig().setDirectory('.')
pipeline.execute(buildType)