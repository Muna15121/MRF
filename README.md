# MRF
# include <windows.h>
#include <GL/glut.h>

void mydisplay()
{
glClear(GL_COLOR_BUFFER_BIT);
glColor3f(0.1,0.1,1.0);
glBegin(GL_POLYGON);
    glVertex2f(0.5, 0.5);
    glVertex2f(-0.5, 0.5);
    glVertex2f(-1, 0);
    glVertex2f(-1, -0.7);
    glVertex2f(1.0, -0.7);
    glVertex2f(1.0, 0);

glEnd();
glFlush();

}
int main(int argc, char** argv)
{
glutInit(&argc,argv);
glutCreateWindow("simple");
glutDisplayFunc(mydisplay);
glutMainLoop();
}
