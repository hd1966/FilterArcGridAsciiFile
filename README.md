# FilterArcGridAsciiFile
Build float[] with vertex positions, normal coordinates and texture coordinates
Usage: 

 CalculateVertex modelLoader = new CalculateVertex ();
 
 String mError= modelLoader.calculateAllData( resourceID,context,SizeofVertexData) 
 
 // size of vertexdata = 10 (vertex positions + normal coordinates + texture coordinates)
 
 if(mError.equals("None")) {//valid format of esri grid ascii file
 
         //if there is not been error load all vertices data (vertex position , normal coordinates, texture coordinates) 
         
         float[] mVerticesData = modelLoader.getAllVerticesData();
         // different attributes in arc grid ascii file can be retrieved  - for example number columns - nCols see below 
        modelLoader.getFl().getAgc().getnCols()...
           ...
To use library in android project add depedency i build.gradle (app level)

implementation 'com.github.hd1966:FilterArcGridAsciiFile:0.1.0'

and add repository in build.gradle (Project level)
 
  maven { url 'https://jitpack.io' }
