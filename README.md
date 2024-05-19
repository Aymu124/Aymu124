// Draw the galaxy
val numStars = 100
val random = Random()
for (i in 0 until numStars) {
    val starRadius = random.nextInt(5) + 1
    val starColor = Color.rgb(random.nextInt(256), random.nextInt(256), random.nextInt(256))
    val starX = random.nextInt(width)
    val starY = random.nextInt(height)
    
    paint.color = starColor
    canvas.drawCircle(starX.toFloat(), starY.toFloat(), starRadius.toFloat(), paint)
}
