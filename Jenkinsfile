node (master){
	
	def buildInfo

	stage('Migrate to DEV'){
		buildInfo = rtGradle.run rootDir: "C:\\Users\\julio.alexandre.melo\\Desktop\\gradle", buildFile: 'build.gradle', tasks: 'gradle task dev update'
	
	}

	stage('Migrate to QA'){
		buildInfo = rtGradle.run rootDir: "C:\\Users\\julio.alexandre.melo\\Desktop\\gradle", buildFile: 'build.gradle', tasks: 'gradle task qa update'
	}

	stage('Migrate to PROD'){
		buildInfo = rtGradle.run rootDir: "C:\\Users\\julio.alexandre.melo\\Desktop\\gradle", buildFile: 'build.gradle', tasks: 'gradle task prod update'
	}

}