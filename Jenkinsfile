node {
  stage 'Run JMeter Test'
  //sh '/usr/local/bin/jmeter -n -t /usr/local/bin/Jenkins_demo1.jmx -l test.jtl'
  sh '/usr/local/bin/jmeter -n -t /usr/local/bin/testplan.jmx -Jusers=250 -l test1.jtl -e -o /usr/local/bin/test'
  perfReport compareBuildPrevious: true, errorFailedThreshold: 10, errorUnstableThreshold: 0, excludeResponseTime: true, modePerformancePerTestCase: true, modeThroughput: true, sourceDataFiles: 'test786.jtl
}
