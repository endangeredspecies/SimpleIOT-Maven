node{
  stage ('cloning the repository'){
	git 'https://github.com/endangeredspecies/SimpleIOT-Maven.git'
  }
  stage ("running appscan on cloud"){
      appscan application: '18f3c3ca-a689-e811-ad5d-00259057d989', credentials: 'ibm_asoc', name: 'test_scm_0730', scanner:static_analyzer('/var/jenkins_home/jobs/test_appscan_on_cloud_pipeline/workspace/test_pipeline_scm'), type: 'Static Analyzer'
  }
}
