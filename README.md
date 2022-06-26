void AimAtPos(float x, float y)
        {
            //By fredaikis
            float ScreenCenterX = (this.Width / 2);
            float ScreenCenterY = (this.Height / 2);
            float TargetX = 0;
            float TargetY = 0;
            if (x != 0)
            {
                if (x > ScreenCenterX)
                {
                    TargetX = -(ScreenCenterX - x);
                    TargetX /= AimSpeed;
                    if (TargetX + ScreenCenterX > ScreenCenterX * 2) TargetX = 0;
                }
 
                if (x < ScreenCenterX)
                {
                    TargetX = x - ScreenCenterX;
                    TargetX /= AimSpeed;
                    if (TargetX + ScreenCenterX < 0) TargetX = 0;
                }
            }
            if (y != 0)
            {
                if (y > ScreenCenterY)
                {
                    TargetY = -(ScreenCenterY - y);
                    TargetY /= AimSpeed;
                    if (TargetY + ScreenCenterY > ScreenCenterY * 2) TargetY = 0;
                }
 
                if (y < ScreenCenterY)
                {
                    TargetY = y - ScreenCenterY;
                    TargetY /= AimSpeed;
                    if (TargetY + ScreenCenterY < 0) TargetY = 0;
                }
            }
            if (!smooth)
            {
                mouse_event(0x0001, (uint)(TargetX), (uint)(TargetY), NULL, NULLPTR);
                return;
            }
            TargetX /= 10;
            TargetY /= 10;
            if (Math.Abs(TargetX) < 1)
            {
                if (TargetX > 0)
                {
                    TargetX = 1;
                }
                if (TargetX < 0)
                {
                    TargetX = -1;
                }
            }
            if (Math.Abs(TargetY) < 1)
            {
                if (TargetY > 0)
                {
                    TargetY = 1;
                }
                if (TargetY < 0)
                {
                    TargetY = -1;
                }
            }
            mouse_event(0x0001, (uint)TargetX, (uint)TargetY, NULL, NULLPTR);
        }Vector3 head = GetBonePos(ent, 51);
if (w2scn(head, w2sHead))
{
    //whatever you want
    if (aimbot && entityTeam != PlayerTeam)
    {
        double distance = Dist2D((this.Width / 2), (this.Height / 2), w2sHead.x, w2sHead.y);
        if (distance < lowDist)
        {
            lowDist = distance;
            aimPosX = W2SNPos.x;
            aimPosY = W2SNPos.y;
        }
    }
    //whatever you want
}void AimAtPos(float x, float y)
        {
            //By fredaikis
            float ScreenCenterX = (this.Width / 2);
            float ScreenCenterY = (this.Height / 2);
            float TargetX = 0;
            float TargetY = 0;
            if (x != 0)
            {
                if (x > ScreenCenterX)
                {
                    TargetX = -(ScreenCenterX - x);
                    TargetX /= AimSpeed;
                    if (TargetX + ScreenCenterX > ScreenCenterX * 2) TargetX = 0;
                }
 
                if (x < ScreenCenterX)
                {
                    TargetX = x - ScreenCenterX;
                    TargetX /= AimSpeed;
                    if (TargetX + ScreenCenterX < 0) TargetX = 0;
                }
            }
            if (y != 0)
            {
                if (y > ScreenCenterY)
                {
                    TargetY = -(ScreenCenterY - y);
                    TargetY /= AimSpeed;
                    if (TargetY + ScreenCenterY > ScreenCenterY * 2) TargetY = 0;
                }
 
                if (y < ScreenCenterY)
                {
                    TargetY = y - ScreenCenterY;
                    TargetY /= AimSpeed;
                    if (TargetY + ScreenCenterY < 0) TargetY = 0;
                }
            }
            if (!smooth)
            {
                mouse_event(0x0001, (uint)(TargetX), (uint)(TargetY), NULL, NULLPTR);
                return;
            }
            TargetX /= 10;
            TargetY /= 10;
            if (Math.Abs(TargetX) < 1)
            {
                if (TargetX > 0)
                {
                    TargetX = 1;
                }
                if (TargetX < 0)
                {
                    TargetX = -1;
                }
            }
            if (Math.Abs(TargetY) < 1)
            {
                if (TargetY > 0)
                {
                    TargetY = 1;
                }
                if (TargetY < 0)
                {
                    TargetY = -1;
                }
            }
            mouse_event(0x0001, (uint)TargetX, (uint)TargetY, NULL, NULLPTR);
        }void AimAtPos(float x, float y)
        {
            //By fredaikis
            float ScreenCenterX = (this.Width / 2);
            float ScreenCenterY = (this.Height / 2);
            float TargetX = 0;
            float TargetY = 0;
            if (x != 0)
            {
                if (x > ScreenCenterX)
                {
                    TargetX = -(ScreenCenterX - x);
                    TargetX /= AimSpeed;
                    if (TargetX + ScreenCenterX > ScreenCenterX * 2) TargetX = 0;
                }
 
                if (x < ScreenCenterX)
                {
                    TargetX = x - ScreenCenterX;
                    TargetX /= AimSpeed;
                    if (TargetX + ScreenCenterX < 0) TargetX = 0;
                }
            }
            if (y != 0)
            {
                if (y > ScreenCenterY)
                {
                    TargetY = -(ScreenCenterY - y);
                    TargetY /= AimSpeed;
                    if (TargetY + ScreenCenterY > ScreenCenterY * 2) TargetY = 0;
                }
 
                if (y < ScreenCenterY)
                {
                    TargetY = y - ScreenCenterY;
                    TargetY /= AimSpeed;
                    if (TargetY + ScreenCenterY < 0) TargetY = 0;
                }
            }
            if (!smooth)
            {
                mouse_event(0x0001, (uint)(TargetX), (uint)(TargetY), NULL, NULLPTR);
                return;
            }
            TargetX /= 10;
            TargetY /= 10;
            if (Math.Abs(TargetX) < 1)
            {
                if (TargetX > 0)
                {
                    TargetX = 1;
                }
                if (TargetX < 0)
                {
                    TargetX = -1;
                }
            }
            if (Math.Abs(TargetY) < 1)
            {
                if (TargetY > 0)
                {
                    TargetY = 1;
                }
                if (TargetY < 0)
                {
                    TargetY = -1;
                }
            }
            mouse_event(0x0001, (uint)TargetX, (uint)TargetY, NULL, NULLPTR);
        }void AimAtPos(float x, float y)
        {
            //By fredaikis
            float ScreenCenterX = (this.Width / 2);
            float ScreenCenterY = (this.Height / 2);
            float TargetX = 0;
            float TargetY = 0;
            if (x != 0)
            {
                if (x > ScreenCenterX)
                {
                    TargetX = -(ScreenCenterX - x);
                    TargetX /= AimSpeed;
                    if (TargetX + ScreenCenterX > ScreenCenterX * 2) TargetX = 0;
                }
 
                if (x < ScreenCenterX)
                {
                    TargetX = x - ScreenCenterX;
                    TargetX /= AimSpeed;
                    if (TargetX + ScreenCenterX < 0) TargetX = 0;
                }
            }
            if (y != 0)
            {
                if (y > ScreenCenterY)
                {
                    TargetY = -(ScreenCenterY - y);
                    TargetY /= AimSpeed;
                    if (TargetY + ScreenCenterY > ScreenCenterY * 2) TargetY = 0;
                }
 
                if (y < ScreenCenterY)
                {
                    TargetY = y - ScreenCenterY;
                    TargetY /= AimSpeed;
                    if (TargetY + ScreenCenterY < 0) TargetY = 0;
                }
            }
            if (!smooth)
            {
                mouse_event(0x0001, (uint)(TargetX), (uint)(TargetY), NULL, NULLPTR);
                return;
            }
            TargetX /= 10;
            TargetY /= 10;
            if (Math.Abs(TargetX) < 1)
            {
                if (TargetX > 0)
                {
                    TargetX = 1;
                }
                if (TargetX < 0)
                {
                    TargetX = -1;
                }
            }
            if (Math.Abs(TargetY) < 1)
            {
                if (TargetY > 0)
                {
                    TargetY = 1;
                }
                if (TargetY < 0)
                {
                    TargetY = -1;
                }
            }
            mouse_event(0x0001, (uint)TargetX, (uint)TargetY, NULL, NULLPTR);
        }
