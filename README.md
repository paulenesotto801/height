# height
/**
 * Calculates the height of an object.
 * 
 * @param {number} width - The width of the object.
 * @param {number} aspectRatio - The aspect ratio of the object.
 * @returns {number} The height of the object.
 */
function calculateHeight(width, aspectRatio) {
  try {
    // Check if both arguments are numbers
    if (typeof width !== 'number' || typeof aspectRatio !== 'number') {
      throw new TypeError('Both arguments must be numbers');
    }
    
    // Calculate and return the height
    return width / aspectRatio;
  } catch (error) {
    // Log the error
    console.error('Error:', error);
    return 0;
  }
}
