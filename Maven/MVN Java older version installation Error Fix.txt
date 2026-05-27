* MVN Java older version installation *
***************************************

(From newer to older in aws Linux)

sudo yum install java-1.8.0-openjdk-devel -y

sudo alternatives --config java

sudo alternatives --config javac

sudo update-alternatives --config javac

mvn --version (check Once)

export JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto.x86_64
export PATH=$JAVA_HOME/bin:$PATH

echo $JAVA_HOME

mvn -version

-- DONE --

===================================================
