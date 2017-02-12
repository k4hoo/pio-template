# pio-template

trait MyQuerySerializer extends CustomQuerySerializer {
  @transient override lazy val querySerializer = org.json4s.DefaultFormats ++ org.json4s.ext.JodaTimeSerializers.all 
}

class Algo extends P2LAlgorithm with MyQuerySerializer ...
