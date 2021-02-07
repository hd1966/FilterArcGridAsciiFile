# FilterArcGridAsciiFile
Build float[] with vertex positions, normal coordinates and texture coordinates
Usage: 
 CalculateVertex modelLoader = new CalculateVertex ();
 String mError= modelLoader.calculateAllData( resourceID,context,SizeofVertexData) // 
 if(mError.equals("None")) {//valid format of esri grid ascii file
            //if there is not been error load all vertices data (vertex position , normal coordinates, texture coordinates) 
             float[] mVerticesData = modelLoader.getAllVerticesData();
            ...
